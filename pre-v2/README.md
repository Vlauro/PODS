# PODS pre-v2 Ontologies

This folder contains the legacy versions of the PODS ontology released before PODS2.

These files are preserved for reference, reproducibility, and compatibility with previous publications. For current implementations, please refer to the main repository README and to the PODS2 ontology files available in the root folder.

## Legacy files included in this folder

- `PODS_0.844.owl`
- `PODS_03.owl`
- `PODS-CORE.owl`

---

# PODS Ontologies

This repository contains three OWL ontologies developed as part of the PODS project (Protocol of Ontological Digital Survey), aimed at formalizing the metadata structure of 3D survey workflows for cultural heritage documentation. Each file corresponds to a specific stage or scope of development:

## PODS_0.844.owl

Purpose: Optimized, reduced version of the PODS ontology designed for use in Omeka-S environments.

Content: Includes only the classes and properties needed to describe 3D Digital Twin Catalogue Records, especially for publishing outputs, such as mesh models, point clouds, URLs, and survey metadata.

Status: This is the most lightweight and deployment-friendly version, tailored for RDF export and practical integration in digital catalogues.

## PODS_03.owl

Purpose: Full and modular version of the PODS ontology for comprehensive semantic representation of photogrammetric workflows.

Content: Includes the entire set of PODS classes, properties, and alignments with reference ontologies such as CIDOC CRM, CRMdig, SKOS, QUDT, and OWL-Time.

Status: Designed for completeness, academic use, and formal reasoning over all phases of the survey process, including acquisition, processing, modelling, and exporting.

## PODS-CORE.owl

Purpose: Merged, rationalized version that combines the essential elements from both PODS_0.844 and PODS_03, structured for public dissemination and semantic interoperability.

Content: Balances expressiveness and implementation-readiness. Retains the core PODS classes and properties while simplifying redundant structures. Fully URI-compliant and aligned with semantic web standards.

Status: This is the stable core release intended for linked data applications, public SPARQL endpoints, and integration with external knowledge graphs.
