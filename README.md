<div align="center">
  <img src="https://ai4eosc.eu/wp-content/uploads/sites/10/2022/09/horizontal-transparent.png" alt="logo" width="500"/>
</div>

# AI4OS Provenance catalog

[![Updated submodules](https://github.com/ai4os/ai4-provenance/actions/workflows/main.yml/badge.svg)](https://github.com/ai4os/ai4-provenance/actions/workflows/main.yml)

This is a catalog for the different AI4OS provenance components:

* [ai4-prov-api](https://github.com/ai4os/ai4-prov-api): Backend for the provenance component
* [ai4-prov-viz](https://github.com/ai4os/ai4-prov-viz): Frontend for the provenance component

The provenance component is currently deployed at: https://provenance.services.ai4os.eu/
Relevant subroutes:

* `GET /?applicationId=<module-id>`: visualize the provenance graph
* `POST /v0/metadata`: trigger the provenance chain (manually providing sources)
* `POST /metadata`: trigger the provenance chain (sources are fetched automatically from `ai4-metadata.yml`)
* `GET /rdf`: retrieve provenance data in RDF format
* `GET /rdf-date` retrieve the creation date of the RDF file
* `GET /rdf-graph`: retrieve graph structure