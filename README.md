PODS Ontologies

This repository contains three OWL ontologies developed as part of the PODS project (Protocol of Ontological Digital Survey), aimed at formalizing the metadata structure of 3D survey workflows for cultural heritage documentation. Each file corresponds to a specific stage or scope of development:

🔹 PODS_0.844.owl

Purpose:
Optimized, reduced version of the PODS ontology designed for use in Omeka-S environments.
Content:
Includes only the classes and properties needed to describe 3D Digital Twin Catalogue Records, especially for publishing outputs (e.g., mesh models, point clouds, URLs, survey metadata).
Status:
This is the most lightweight and deployment-friendly version, tailored for RDF export and practical integration in digital catalogues.

🔹 PODS_03.owl

Purpose:
Full and modular version of the PODS ontology for comprehensive semantic representation of photogrammetric workflows.
Content:
Includes the entire set of PODS classes (F1–F5 and sub-classes), properties (Y1–Y95), and alignments with reference ontologies such as CIDOC CRM, CRMDig, SKOS, QUDT, OWL-Time.
Status:
Designed for completeness, academic use, and formal reasoning over all phases of the survey process (acquisition, processing, modelling, exporting).

🔹 PODS-CORE.owl

Purpose:
Merged, rationalized version that combines the essential elements from both PODS_0.844 and PODS_03, structured for public dissemination and semantic interoperability.
Content:
Balances expressiveness and implementation-readiness. Retains the core PODS classes and properties while simplifying redundant structures. Fully URI-compliant and aligned with semantic web standards.
Status:
This is the stable core release intended for linked data applications, public SPARQL endpoints, and integration with external knowledge graphs.
