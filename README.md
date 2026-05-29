# PODS Ontology

**PODS** (*Protocol of Ontological Digital Survey*) is an ontology designed to formalize and document the digital surveying workflow, with particular attention to the semantic description, management, and preservation of cultural heritage through structured metadata.

PODS was developed as a refinement and extension of previous protocols such as **BeAPG** and **FOPPA**. Its main purpose is to provide an **event-oriented** and semantically coherent framework for representing the metadata of 3D digital survey workflows, including acquisition, processing, modelling, exporting, and final use of Digital Twins and related digital objects. In this perspective, the survey workflow is described as a chain of events whose parameters, tools, actors, and outputs can be explicitly documented and connected.

The ontology integrates and aligns with established semantic standards such as **SKOS**, **QUDT**, **CIDOC CRM**, and **CIDOC CRMdig**, in order to enhance interoperability, controlled vocabulary management, and compatibility with international data-sharing and linked data environments.

## PODS and PODS2

**PODS** is the conceptual framework.  
**PODS2** is the current OWL implementation released in this repository.

## Current Version: PODS2

The current version of the ontology is **PODS2**.

The complete ontology is provided as:

### `PODS2.owl`

This file contains the full structure of the PODS ontology, including the classes and properties required to describe the lifecycle of a Digital Twin, from the initial survey object and acquisition activities to processing, modelling, exporting, dissemination, and final use.

## Modular Structure

PODS2 is organized into four main compositional modules. Each module corresponds to one of the main workflow phases treated in PODS as top-level events of the digital survey process, and is also available as an independent OWL file.

The modular structure is intended to support both full ontology use and phase-specific implementation.

### PODS2 Acquisition Module

**File:**  
`PODS2-AcquisitionModule.owl`

This module describes the **acquisition** phase of a digital survey. It includes classes and properties related to the surveyed object, acquisition event, acquisition devices, software, operators, acquisition methods, trajectories, raw data, image sets, acquisition places, dates, coordinates, calibration tools, eidotypes, and acquisition environments.

### PODS2 Processing Module

**File:**  
`PODS2-ProcessingModule.owl`

This module describes the **processing** phase of a digital survey. It includes classes and properties related to acquisition input, processing devices, processing software, operators, matching, densification, point clouds, densified point clouds, calibration, alignment, registration, measurements, and processing descriptions.

### PODS2 Modelling Module

**File:**  
`PODS2-ModellingModule.owl`

This module describes the **modelling** phase of a digital survey. It includes classes and properties related to mesh reconstruction, texturing, modifying mesh, modelling devices, modelling software, modelling operators, reconstruction methods, texturing methods, digital scale, smoothing filters, texture sets, scaling factors, 3D meshes, textured 3D meshes, and the creation of Digital Twins.

### PODS2 Exporting Module

**File:**  
`PODS2-ExportingModule.owl`

This module describes the **exporting** phase of a digital survey. It includes classes and properties related to the final use of Digital Twins and 3D models, including video rendering, 3D printing, GIS integration, CAD analysis, prospectuses, research outputs, interactive environments, database implementation, AR/MR applications, interrogation tools, and physical or digital carriers.

## Ontology Structure

Each class and property in PODS follows a structured documentation model.

Classes are identified through a sequential naming convention, such as **F1**, **F2**, **F3**, and so on. Properties are identified through a corresponding **Y** numbering system. This structure supports internal consistency and allows each element of the ontology to be connected to a specific phase, event, or action within the digital survey workflow.

Each ontology element may include:

- a label  
- a URI  
- superclass or subclass relations  
- domain and range, where applicable  
- a scope note  
- examples of use  
- alignment with reference ontologies  
- descriptive metadata  

The goal of this structure is to ensure consistency, accuracy, traceability, and semantic interoperability in the documentation of 3D digital heritage assets.

## Legacy Versions before PODS2

Previous versions of the PODS ontology are preserved for reference, reproducibility, and compatibility with earlier publications.

They are available in the folder:

### `pre-v2/`

This folder contains earlier ontology files and the previous README structure, including:

- `PODS_0.844.owl`
- `PODS_03.owl`
- `PODS-CORE.owl`

These files are maintained as **legacy versions** and should be cited or used only when referring to work developed before the release of PODS2.

For new implementations, use **PODS2.owl** or one of the four **PODS2 module files**.
