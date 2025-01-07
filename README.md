PODS 1_1_7

Protocol of Ontological Digital Survey 

Introduction to the PODS Ontology

The Protocol of Ontological Digital Survey (PODS) is an ontology designed to standardize and formalize the digital surveying process, particularly for the documentation and preservation of cultural heritage. Developed as a refinement and expansion of previous protocols such as BeAPG and FOPPA, PODS focuses on the precise metadata representation of each step in the digital surveying workflow, ensuring a structured and semantically coherent approach to 3D data acquisition, processing, and management.

The ontology integrates established standards such as SKOS, QUDT, and CIDOC-CRM, with specific extensions like CIDOC-CRMdig, to enhance interoperability and compatibility with international data-sharing platforms, including Wikimedia’s database structures. PODS provides a robust framework for representing the phases, sub-phases, actions, and tools involved in digital surveying, facilitating the creation of accurate, structured data about three-dimensional cultural heritage assets.

The ontology is organized into classes and properties that define and describe the key components of the digital surveying process. These classes capture essential information about the objects, processes, and tools used in 3D photogrammetry, enabling the precise cataloging of digital models, point clouds, and related metadata. PODS aims to create a scalable, adaptable system that can be applied in diverse contexts, from archaeological excavation sites to museum digitalization projects.

This document presents the detailed structure of the PODS ontology, outlining each class and its associated properties, along with their relationships to established standards. The goal is to provide a clear and systematic framework that ensures consistency, accuracy, and completeness in digital heritage documentation.

Each class in the PODS ontology follows a precise structure. The name is designated using a sequential format (e.g., F1, F2), which establishes a hierarchical relationship among the classes based on their connection to the overall process. Next is the URI, the unique HTTP address of each class and property, treated as individual knowledge items and stored within a database structured in Omeka Classic architecture. Following this is the classification of the class, indicating if it is a subclass of another class, specifying the parent class where applicable. For properties, this section also specifies the Domain and Range.

The structure then includes the "Scope Note," which provides a detailed description of the class or property and clarifies its intended purpose. Examples of usage are provided to illustrate real-world applications. After this is the "Label," which defines how the class is referenced, following a naming convention that associates various elements with the digital acquisition phases they are related to. Finally, the "dc description " indicates the class’s categorization according to metadata legitimacy standards, with a reference to the relevant metadata classification category for further context.


Class Declaration 

PODS
F1 Survey Object
F2 Acquisition
F3 Processing
F4 Modelling
F5 Exporting
F6 Acquisition Raw Data
F7 Picture Set
F8 Picture
F9 Acquisition Device
F10 Processing Device
F11 Modelling Device
F12 Acquisition Trajectory
F13 Acquisition Method
F14 Matching Method
F15 Recontruction Method
F16 Texturing Method
F17 Acquisition Trajectory Type
F18 Dominant Geometry Type
F19 Scale Type
F20 Acquisition Device Type
F21 Matching Algorithm Type
F22 Densification Algorithm Type
F23 Reconstruction Algorithm Type
F24  Texturing Type
F25 Acquisition Raw Data
F26 Point Cloud
F27 Densified Point Cloud
F28 3D Mesh
F29 Textured 3D Mesh
F30 Acquisition Software
F31 Processing Software
F32 Modelling Software
F33 Acquisition Phase
F34 Processing Phase
F35 Raw Data Carrier
F36 Picture Carrier
F37 Survey Operator
F38 Processing Operator
F39 Modelling Operator
F40 Eydotipe
F41 Number of Picture
F42 Place Of Acquisition
F43 Survey Date
F44 Acquisition Description
F45  Acquisition Coordinates
F46  Matching
F47  Densification
F48 Densification Method
F49  Near Sampling Points Range_SFM Point Seeds
F50 Point Cloud Measurement
F51 Point Cloud Number of Point
F52 Dense Point Cloud Measurement
F53 Dense Point Cloud Number of Point
F54 Point Cloud Vertex Quality
F55 Depth Noise Filtering
F56 Mesh Reconstruction
F57 Texturing Mesh
F58 Modifying Mesh
F100 3D Digital Twin
F59 Digital Scale
F60 Smoothing Filter
F61 Color Balance/Multiband Texture
F62 Texture Set of 3D Mesh
F63 Number of Texture
F64 Modelling Description
F65 Modelling Date
F66 Modelling Determination
F67 Modelling Elimination
F68 Digital Twin Physical Carrier
F69 Exporting Description
F70 Number of Final Destination
F71 Final Use of Digital Twin
F72 3D Model Video Rendering
F73 Editing Video
F74 Video Editing Software
F75 Project Video
F76 3D Model for 3D Print
F77 Printing Digital Twin
F78 Material for 3D Printing
F79 Printing Device
F80 Printed Digital Twin
F81 3D Model for G.I.S.
F82 Reference GIS System
F83 GIS Software
F84 3D Model for Prospectus
F85 CAD Analysis
F86 Software CAD
F87 3D Model Prospectus
F88 Archaeometric 3D Model
F89 Project Analysis
F90 Data Log Analysis
F91 Model for Interactive
F92 Interactive Project Implementation
F93 Interactive Software
F94 3D Model for Database
F95 Database Project Implementation
F96 Database Architecture
F97 AR 3D Model
F98 AR/MR Project Implementation
F99 AR Software Modelling
F101: Survey Phase
F102: 3D Digital Asset




F1 Survey Object
URI: https://photogrammetry.altervista.org/items/show/87 
SubClass of CIDC-CRM class
S10 Material Substantial
Scope Note 
Survey Object denotes any object subjected to photogrammetric surveying or any kind of digital surveying. It represents the target of data acquisition processes, crucial for generating detailed digital records, analyses, and reconstructions within the FOPPA model for archaeological documentation. It must be a solid and visible object. The expression visible means that it interacts with light. Where possible Indicate the URL of the official web repository of the object, if it does not exist indicate the unique identification code of the detected object
Examples:
a wild boar jaw AFMNM005 detected with photogrammetric technique at the laboratory of the archaeological museum of Okayama (Japan) coming from the Minamikata excavation in the context of the BeArchaeo project (Lauro, 2019)
A castle surveyed with photogrammetric technique (Artopoulos 2015)
A fresco in a medieval chapel (D. Abate 2016)
 https://www.britishmuseum.org/collection/object/W_1882-0714-509 ( The Babylonian Map of The world, BM92687 )

Label: SurveyObject

dc: description "Relevant for:" teaching and dissemination

—---------------------------------------------------------------------------------------------------------

F2 Acquisition 
URI: https://photogrammetry.altervista.org/items/show/88 
SubClass of CIDC-CRM class
D2 Digitization Process
Scope Note 
Acquisition refers to the process of capturing detailed photographic data of an object or structure. This involves systematically taking overlapping photographs from various angles to create a comprehensive and accurate 3D model, crucial for archaeological documentation and analysis.
Examples:
The photogrammetric survey of a contemporary art sculpture (Ucakar 2022) 
The photogrammetric survey of the walls of Cortona (Lauro 2023)
The survey of the facade of Bedzin Castle using laser scanning and photogrammetry (Klapa 2017)

Label: Acquisition

dc: description "Relevant for:" Conservation and Enhancement 
—-------------------------------------------------------------------------------------------

F3 Processing 
URI: https://photogrammetry.altervista.org/items/show/89 
SubClass of CIDC-CRM class
D7 Digital Machine Event 
Scope Note 
Processing in photogrammetry involves transforming raw data files into usable outputs. This includes validating image quality, stitching photographs, generating 3D models, and correcting errors like texture and polygon mismatches. It ensures data consistency, enhances detail accuracy, and prepares the images for further modeling and analysis in archaeological contexts. This specific action is in a state of dependence on the RawDataFile and on the Acquisition action and although intentional and therefore Activity depends on the choices made in the previous classes.
Examples: 
The processing of photographs of the photogrammetric survey of a wild boar jaw from the Minamikata site (Lauro 2019) 
The processing of Bayman's photographs of the Buddha (A. Gruen 2004)

dc: description "Relevant for:" Archaeometric analysis 

—-------------------------------------------------------------------------------------------

F4 Modelling 
URI: https://photogrammetry.altervista.org/items/show/90 
SubClass of CIDC-CRM class
D7 Digital Machine Event 
Scope Note 
Modeling a 3D model involves creating and refining a digital representation of an object using specialized software. This process includes shaping the geometry, and adding details to achieve an accurate and detailed virtual model, ready for analysis, visualization, or further processing.
This is an activity confined to modeling, not to be confused with the Modeling instructions which already include the construction of the mesh, and which however are continuous with it. The modeling is driven by design and research considerations and has no aesthetic character, distinguishing itself from 3D design modeling, which is not the subject of this analysis.
Example: 
The reconstructive modeling of the Temple of Saturn at the Forum in Rome based on the photogrammetric survey of the structure (Koller 2009)
Mesh processing of an excavation sector of the Oglala National Grassland (Douglas 2015)

Label: Modelling

dc: description "Relevant for:" Conservation and Enhancement 

—-------------------------------------------------------------------------------------------

F5 Exporting
URI: https://photogrammetry.altervista.org/items/show/91 
SubClass of CIDC-CRM class
D7 Digital Machine Event 
Scope Note 
Exporting involves the final stages of digital asset management. This phase encompasses exporting the processed data and archiving it for long-term preservation, ensuring the integrity and accessibility of digital records.
Examples:


Label: Exporting

dc: description "Relevant for:" Archaeometric analysis 

—-------------------------------------------------------------------------------------------

F6 Acquisition Raw Data 
URI: https://photogrammetry.altervista.org/items/show/92 
SubClass of CIDC-CRM class
D1 Digital Object 
Scope Note 
A Raw Data File contains unprocessed image data captured during photogrammetric surveys or digital information acquired by a laser scanner in the acquisition phase and not yet processed or even the raw data of a LiDar survey. This class generally refers to any form of raw data resulting from the processing of a visible object as described in the F1 Survey Object class.. These files preserve original color, detail, and metadata, crucial for accurate 3D model reconstruction. In archaeological contexts, they ensure comprehensive documentation of artifacts and structures, facilitating detailed analysis and interpretation.
Raw Data files are distinguished as "incomplete" Conceptual Objects, in the sense that they are complete in their existence but their function is aimed at the processing which constitutes their reason for being. In photogrammetry it is the photographs that make up the survey.
Examples:


Label: AcquisitionRawData

dc: description "Relevant for:" Archaeometric analysis 
—-------------------------------------------------------------------------------------------

F7 Picture Set 
URI: https://photogrammetry.altervista.org/items/show/93 
SubClass of: 
F6 Acquisition Raw Data
Scope Note:
The Picture Set class refers to a collection of unprocessed digital images captured during the acquisition phase of a photogrammetric survey. These images, taken systematically from multiple viewpoints, are critical for reconstructing 3D models of surveyed objects or environments. Each picture within the set is treated as part of a coherent whole, as the completeness and quality of the survey depend on the collective set rather than individual photographs.
Picture Sets preserve high-resolution details, color information, and metadata essential for subsequent processing stages, ensuring accurate spatial and geometric reconstructions.
Examples: 
Photographs captured for a photogrammetric survey of an archaeological artifact or a historical building.
The 181 photographs that form the photogrammetric survey of the AFMNM005 jaw from the Minamikata excavation (Lauro 2019)
Label: AcquisitionPictureSet

dc: description "Relevant for:" Archaeometric analysis 
—-------------------------------------------------------------------------------------------

F8 Picture 
URI: https://photogrammetry.altervista.org/items/show/94 
SubClass of: 
F7 Picture Set 
Scope Note:
The Picture class represents a single digital photograph taken during the acquisition phase of a photogrammetric survey. Each Picture is an unprocessed image that contributes to the overall Picture Set and is crucial for reconstructing precise 3D models. These photographs capture detailed visual data, including color, texture, and spatial relationships, and serve as foundational raw data for photogrammetric processing. Although each Picture is valuable individually, its full significance is realized when integrated into the entire Picture Set.
Examples:
A single high-resolution image of an archaeological artifact taken from a specific angle as part of a complete photogrammetric survey.
Label: AcquisitionSinglePicture
—-------------------------------------------------------------------------------------------

F9 Acquisition Device 
URI: https://photogrammetry.altervista.org/items/show/95 
SubClass of: 
D8 Digital Device
Scope Note:
The Acquisition Device class represents any digital tool or instrument used during the acquisition phase of a photogrammetric survey or other data collection processes. These devices capture raw data such as photographs, point clouds, or laser scans, which serve as the foundation for subsequent processing and modeling. Examples of Acquisition Devices include digital cameras, 360° cameras, laser scanners, or LiDAR devices. Each device has specific technical capabilities that influence the quality and precision of the data collected, playing a critical role in the accuracy of the final 3D reconstruction.
Examples:
A DSLR camera used to capture high-resolution images during a photogrammetric survey of an archaeological structure.
A LiDAR scanner employed to gather 3D point cloud data from a heritage site.
Label: AcquisitionDevice

dc: description "Relevant for:" Conservation and Enhancement

—-------------------------------------------------------------------------------------------

F10 Processing Device 
URI: https://photogrammetry.altervista.org/items/show/96 
SubClass of: 
D8 Digital Device
Scope Note:
The Processing Device class refers to any digital apparatus responsible for executing the computational tasks involved in the processing phase of data collected during a photogrammetric survey or other types of acquisition. This device typically includes computers running specialized software used to transform raw data (such as images or point clouds) into processed outputs like 3D models or Densified Point Clouds. In certain cases, such as laser scanners or other integrated systems, the same device used for acquisition may also perform data processing. The technical specifications and capabilities of the Processing Device directly influence the efficiency, speed, and quality of the final results.
Examples:
A high-performance computer equipped with photogrammetry software (e.g., Agisoft Metashape or Zephyr) used to process survey images into 3D models.
A laser scanner that both collects and processes point cloud data directly within its onboard system.
Label: ProcessingDevice

dc: description "Relevant for:" Archaeometric analysis 

—-------------------------------------------------------------------------------------------

F11 Modelling Device 
URI: https://photogrammetry.altervista.org/items/show/97 
SubClass of: 
D8 Digital Device
Scope Note:
The Modelling Device class refers to any digital apparatus specifically used to perform the modeling and transformation of 3D models derived from processed data during photogrammetric surveys or other similar workflows. This device is most commonly a high-performance computer equipped with specialized software for 3D modeling, texturing, and refinement of point clouds or meshes. The Modelling Device plays a crucial role in converting raw or processed data into final, high-quality 3D models ready for visualization, analysis, or export. Its processing power and graphic capabilities directly impact the accuracy, level of detail, and speed of the 3D model's refinement.
Examples:
A workstation running 3D modeling software like Blender, Rhino, or Autodesk Maya used for finalizing and optimizing a 3D mesh created from photogrammetry.
A high-spec PC equipped with advanced GPUs to handle complex textures and lighting setups for archaeological 3D models.
Label: ModellingDevice

dc: description "Relevant for:" Archaeometric analysis 

—-------------------------------------------------------------------------------------------

F12 Acquisition Trajectory
URI: https://photogrammetry.altervista.org/items/show/98 
SubClass of: 
E29 Design and Procedure
Scope Note:
The Acquisition Trajectory class refers to the physical path or series of positions followed by an acquisition device (such as a camera or laser scanner) during the data acquisition phase of photogrammetric or other survey processes. This trajectory defines the movement or stationary positions of the device relative to the object or area being documented, affecting the quality, coverage, and accuracy of the data captured. The Acquisition Trajectory can include linear paths, spirals, concentric movements, or modular setups in the case of a laser scanner, depending on the methodology adopted. Accurate documentation of the trajectory is essential for ensuring comprehensive and consistent capture of an object’s geometry, which is vital for subsequent processing and modeling phases.
Examples:
A spiral trajectory executed by a camera as it moves around an archaeological artifact for a photogrammetric survey.
A modular scanning setup, where a laser scanner is placed at different strategic positions around an architectural site to capture comprehensive point cloud data.
Label: AcquisitionPath

dc: description "Relevant for:" Archaeometric analysis 
—-------------------------------------------------------------------------------------------

F13 Acquisition Method 
URI: https://photogrammetry.altervista.org/items/show/99 
SubClass of: 
E29 Design and Procedure
Scope Note:
The Acquisition Method class refers to the set of protocols, guidelines, or operational instructions that dictate how the acquisition process is conducted during a photogrammetric or other survey operation. This class captures the methodology adopted for data capture, specifying procedural elements such as device settings, trajectory planning, object coverage, and environmental considerations. The Acquisition Method can range from formalized protocols, such as the Metashape Manual or the McGlone Method, to custom or ad-hoc procedures defined for specific projects or objects. The choice of method impacts the completeness and quality of the raw data produced, influencing all subsequent phases of processing and modeling.

Examples:
The FOPPA protocol for archaeological photogrammetry, which prescribes specific camera settings and trajectories for artifact documentation.
The McGlone Method, which provides a standardized set of steps for capturing imagery in aerial photogrammetry surveys.
Label: AcquisitionMethod

dc: description "Relevant for:" Restoration
—-------------------------------------------------------------------------------------------

F14 Matching Method 
URI: https://photogrammetry.altervista.org/items/show/100 
SubClass of: 
E29 Design and Procedure
Scope Note:
The Matching Method class refers to the procedures and algorithms employed during the initial processing phase to extract corresponding points from multiple images based on color, texture, or other visual data. This method is essential for generating an accurate point cloud by identifying shared points across photographs or other forms of acquired raw data, such as laser scans. The Matching Method includes techniques like feature detection, keypoint extraction, and descriptor matching, which are critical for aligning images and generating the foundational structure of the 3D model. Various algorithms such as SIFT, SURF, or proprietary methods like those found in Metashape or Zephyr can be classified under this category.
Examples:
Using the SIFT (Scale-Invariant Feature Transform) algorithm to match key points across a series of overlapping photographs in a photogrammetric survey.
Employing a matching algorithm within Zephyr to generate an initial point cloud from high-resolution drone imagery.
Label: Processing_MatchingMethod

dc: description "Relevant for:" Restoration
—-------------------------------------------------------------------------------------------

F15 Reconstruction Method 
URI: https://photogrammetry.altervista.org/items/show/101 
SubClass of: 
E29 Design and Procedure
Scope Note:
The Reconstruction Method class refers to the procedures and algorithms used to transform a densified point cloud into a polygonal mesh, thereby creating a structured 3D representation of an object or scene. This process involves generating polygons, typically triangles or quads, that form the mesh surface based on the spatial data from the point cloud. The Reconstruction Method also includes steps like mesh optimization, hole filling, and refinement to improve accuracy and ensure the continuity of the 3D surface. Different software solutions and algorithms such as Poisson Surface Reconstruction, Delaunay Triangulation, or Ball-Pivoting Algorithm are examples of methods employed during this phase.
Examples:
Applying the Poisson Surface Reconstruction algorithm in Metashape to create a high-fidelity mesh from a dense point cloud.
Using Delaunay Triangulation to generate a watertight 3D mesh in Zephyr from a multi-view photogrammetric survey.
Label: Modelling_ReconstructionMethod

dc: description "Relevant for:" Restoration
—-------------------------------------------------------------------------------------------

F16 Texturing Method 
URI: https://photogrammetry.altervista.org/items/show/102 
SubClass of: 
E29 Design and Procedure
Scope Note:
The Texturing Method class refers to the procedures and algorithms used to map color information onto a 3D mesh, creating a realistic representation by applying textures that enhance the visual fidelity of the model. This process involves associating 2D images (or texture maps) with the 3D geometry of the mesh, either by projecting photographs directly onto the surface or by generating UV maps that accurately correspond to the model’s topology. The Texturing Method ensures that each polygon in the mesh receives appropriate color information from the photographic data, and may also involve steps like blending multiple images to eliminate seams or inconsistencies. Textures can either be embedded in the model file or stored externally, depending on the file format and desired use of the model.
Examples:
Using Metashape's Blended Mapping algorithm to generate a unified texture from multiple photographs.
Applying the UV Mapping technique in Blender to unwrap a mesh and create texture coordinates for an optimized 3D model.
Label: Modelling_TexturingMethod

dc: description "Relevant for:" Archaeometric analysis 

—-------------------------------------------------------------------------------------------

F17 Acquisition Trajectory Type 
URI: https://photogrammetry.altervista.org/items/show/103 
SubClass of: 
E55 Type
Scope Note:
The Acquisition Trajectory Type class encompasses the various classifications of movement patterns executed by the acquisition device during the data collection process. These types are essential for understanding the methodology of data capture and are critical for accurately interpreting the resulting raw data. Different trajectory types can include linear movements, spiral paths, vertical scans, and other systematic approaches tailored to the specific context of the survey. Each trajectory type informs the photogrammetric workflow by dictating how the acquisition device interacts with the subject, which ultimately affects the quality and detail of the captured data.
Examples:
Spiral Trajectory: Movement around the subject in a circular path to capture detailed data from all angles.
Linear Trajectory: Straightforward movement along a defined line to ensure consistent coverage of the object.
Vertical Scan: Upward or downward movements intended to gather data from different height levels of the subject.
Label: AcquisitionPath/TrajectoryTypology

dc: description "Relevant for:" Restoration

—-------------------------------------------------------------------------------------------
F18 Dominant Geometry Type 
URI: https://photogrammetry.altervista.org/items/show/104 
SubClass of: 
E55 Type
Scope Note:
The Dominant Geometry Type class refers to the primary geometric form of the surveyed object, conceptualized as the essential shape to which the object can be reduced. This classification aligns with specific reference thesauri, such as the FOPPA Geometry Thesaurus, which delineates these forms based on the principle that the dominant geometry is determined by the conjunction of the opposite vertices of the object, considering an approximation that does not exceed a 45-degree inclination of the faces. 
Examples:
Sphere: A basketball, characterized by its round shape.
Cylinder: A bottle, defined by its elongated form.
Parallelepiped: A book, reduced to its rectangular prism shape.
Bowl/Hemisphere: A κρατήρ, represented as a hemispherical shape.
Approximate Geometry: An irregular glass bead as a sphere, a ceramic shard or animal jaw as a parallelepiped, a column as a cylinder, and a crater or lake as hemispherical.
Label: AcquisitionGeometryTypology

dc: description "Relevant for:" Archaeometric analysis 

—-------------------------------------------------------------------------------------------

F19 Scale Type 
URI: https://photogrammetry.altervista.org/items/show/105 
SubClass of: 
E55 Type
Scope Note:
The Scale Type class pertains to the classification of the size of an object according to various available thesauri. This classification reflects the volume of the object and, depending on the thesaurus employed, may also relate to its functional characteristics. This class serves as a basis for understanding the object's scale in relation to its volume and, when applicable, its function according to the selected thesaurus.  Where possible expressed according to the following scheme:

Scale of the Surveyed Object:
A: Small object (equal to or smaller than 1 cm)
B: Medium Object (1cm to 30cm)
C: Large Object (from 30 cm upwards)
Q: Open architectural structure
E: Architectural element (part of an architectural structure)
F: Cave or underground structure
G: Landscape element

and expressed according to the measurement of the ideal bounding box in mm
Length, Width followed by Height which will respond to the Geosparql property
 geo:hasSize

https://docs.ogc.org/is/22-047r1/22-047r1.html#_property_geohhassize

Examples: 
Small Object: Equal to or smaller than 1 cm (FOPPA).
Medium Object: Ranging from 1 cm to 30 cm (FOPPA)
Open Architectural Structure: Entire buildings or significant structures (FOPPA).
Bend (COSCHKR)
Corner  (COSCHKR)
Joint  (COSCHKR)
Label: AcquisitionScaleObjectType

dc: description "Relevant for:" teaching and dissemination
—-------------------------------------------------------------------------------------------

F20 Acquisition Device Type  
URI: https://photogrammetry.altervista.org/items/show/106 
SubClass of: 
E55 Type
Scope Note:
The Acquisition Device Type class refers to the various types of acquisition instruments used in photogrammetry and surveying, such as cameras, laser scanners, and LiDAR systems. This class is essential for categorizing and managing the different instruments employed for data capture in archaeological documentation.
Examples:
Camera: Standard photographic equipment for capturing images.
Laser Scanner: Device used for capturing 3D data of surfaces through laser measurements.
LiDAR: Technology that measures distances by illuminating a target with laser light and analyzing the reflected light.
Total Station: An optical/electronic instrument used for surveying and building construction.
Handheld Scanners: Portable devices for capturing detailed surface information.
Label: AcquisitionDeviceType

dc: description "Relevant for:" Conservation and Enhancement 
—-------------------------------------------------------------------------------------------

F21 Matching Algorithm Type  
URI: https://photogrammetry.altervista.org/items/show/107 
SubClass of: 
E55 Type
Scope Note:
The Matching Algorithm Type class encompasses the various types of algorithms utilized for extracting the initial point cloud from images in photogrammetry or from positional information in laser scanning. This class is crucial for categorizing the different methodologies employed in point cloud generation.
Examples:
Feature Matching: Algorithms that identify and match distinctive features in overlapping images.
Stereo Matching: Techniques that derive depth information from two or more images taken from different viewpoints.
Structure from Motion (SfM): Algorithms that reconstruct 3D structures from a series of 2D images.
Depth Map Algorithms: Methods that generate depth information from laser scanner data.
Label: Processing_MatchingAlgorithmType

dc: description "Relevant for:" Archaeometric analysis
—-------------------------------------------------------------------------------------------

F22 Densification Algorithm Type  
URI: https://photogrammetry.altervista.org/items/show/108 
SubClass of: 
E55 Type
Scope Note:
The Densification Algorithm Type class refers to the various types of algorithms used to obtain a densified point cloud from an initial point cloud. These algorithms enhance the resolution and detail of the point cloud, making it more suitable for detailed analysis and modeling.
Examples:
Point Cloud Densification: Algorithms that interpolate additional points between existing points to increase density.
Multi-View Densification: Methods that utilize multiple images to enhance point cloud density through additional data capture.
Depth Map Fusion: Algorithms that combine depth maps from multiple scans to create a denser point cloud.
Regularization Techniques: Approaches that improve point distribution and reduce noise in the densified point cloud.
Label: Processing_DensificationAlgorithmType

dc: description "Relevant for:" Archaeometric analysis

—-------------------------------------------------------------------------------------------

F23 Reconstruction Algorithm Type 
URI: https://photogrammetry.altervista.org/items/show/109 
SubClass of: 
E55 Type
Scope Note:
The Reconstruction Algorithm Type class refers to the various types of algorithms used to create a mesh or surface from a point cloud. These algorithms transform the discrete points into a continuous representation, facilitating the modeling and visualization of 3D objects.

Examples:
Triangulation Algorithms: Techniques that connect points in the point cloud to form triangular meshes.
Poisson Surface Reconstruction: A method that generates a smooth surface by solving a Poisson equation based on point cloud data.
Alpha Shapes: Approaches that create a mesh based on the shape and distribution of points, defining boundaries for the reconstructed surface.
Delaunay Triangulation: Algorithms that maximize the minimum angle of triangles in the mesh, ensuring quality and even distribution of mesh elements.
Incremental Surface Reconstruction: Techniques that progressively build the surface by adding points and connecting them as more data becomes available.
Label: Modelling_ReconstructionAlgorithmType

dc: description "Relevant for:" Archaeometric analysis 
—-------------------------------------------------------------------------------------------

F24 Texturing Type 
URI: https://photogrammetry.altervista.org/items/show/110 
SubClass of: 
E55 Type
Scope Note:
The Texturing Type class refers to the various techniques, algorithms, or methods used to create textures for 3D models. These processes enhance the visual detail of models by applying color, patterns, and surface characteristics that mimic real-world appearances.

Examples:
UV Mapping: A technique that involves projecting a 2D image onto a 3D model by mapping its surface coordinates to texture coordinates.
Bump Mapping: An algorithm that simulates surface detail by altering the lighting of a model without changing its geometry, giving the illusion of depth.
Normal Mapping: Similar to bump mapping, this technique uses a normal map to create detailed surface features by modifying the surface normals of the geometry.
Procedural Texturing: Methods that generate textures algorithmically rather than using bitmap images, allowing for dynamic and complex surface appearances.
Texture Painting: The process of manually painting textures directly onto the 3D model within specialized software, allowing for artistic control and customization.
Label: Modelling_TexturingType

dc: description "Relevant for:" Archaeometric analysis 

—-------------------------------------------------------------------------------------------

F25 Acquisition Raw Data  
URI: https://photogrammetry.altervista.org/items/show/111 
SubClass of: 
D9 Data Object
Scope Note:
The Acquisition Raw Data class refers to the unprocessed data resulting from the acquisition phase of photogrammetric surveys or laser scanning. These data serve as the foundational elements for subsequent processing steps and are essential for creating accurate 3D models. The raw data maintain original details and metadata critical for ensuring fidelity in model reconstruction.
Examples:
Unedited images captured by a camera during a photogrammetric survey.
Raw laser scan data collected from a laser scanner without any preprocessing.
LiDAR point cloud data that has not undergone filtering or classification.
Initial digital information files that contain unprocessed sensor readings from acquisition devices.
Label: AcquiredRawData

dc: description "Relevant for:" Archaeometric analysis 


—-------------------------------------------------------------------------------------------

F26 Point Cloud  
URI: https://photogrammetry.altervista.org/items/show/112 
SubClass of: 
D9 Data Object
Scope Note:
The Point Cloud class represents the initial output generated from the processing of raw data in photogrammetry or laser scanning. This class includes unrefined sets of data points that define the three-dimensional spatial distribution of the scanned object. The point cloud is a crucial intermediary stage prior to any densification processes, providing a preliminary representation of the object's surface geometry.
Examples:
A collection of 3D points representing the surface of an archaeological artifact as captured from raw data.
Initial point cloud data generated from a laser scanner before any further processing steps.
Sparse point data that outlines the basic shape and features of an object without refinement.
The set of points collected from an acquisition with a total station placed in relation in a coordinate grid
Label: ProcessedPointCloud

dc: description "Relevant for:" Conservation and Enhancement 

—-------------------------------------------------------------------------------------------

F27 Densified Point Cloud 
URI: https://photogrammetry.altervista.org/items/show/113 
SubClass of: 
D9 Data Object
Scope Note:
The Densified Point Cloud class refers to a refined set of three-dimensional data points that have undergone an additional processing stage to enhance point density. This process occurs independently from the initial matching phase and results in a more detailed representation of the object's surface geometry. Densified point clouds are crucial for improving the accuracy and quality of subsequent modeling and visualization tasks. Where possible expressed with a URL to the viewer or the repository where the densified point cloud is located

Examples:
A point cloud obtained after applying algorithms that increase the density of points to capture finer details of an archaeological site.
Densified point data generated from a laser scanner, where additional points are added to improve spatial resolution.
A processed point cloud used for advanced analysis and 3D reconstruction, characterized by a higher density of points compared to the initial output.
Enhanced point cloud data created through interpolation techniques to fill gaps in the original point set.
https://openheritage3d.org/project.php?id=7ymp-ta22 
Label: ProcessedDensifiedPointCloud

dc: description "Relevant for:" teaching and dissemination

—-------------------------------------------------------------------------------------------

F28 3D Mesh 
URI: https://photogrammetry.altervista.org/items/show/114 
SubClass of: 
D9 Data Object
Scope Note:
The 3D Mesh class refers to a three-dimensional model constructed from a densified point cloud. This mesh represents the geometric structure of the object and is generated prior to any texturing processes. It includes the surface topology and spatial relationships derived solely from the point cloud data, making it essential for visualizing the basic form and structure of the scanned object before adding detailed textures.

Examples:
A geometric representation of an archaeological artifact created from a densified point cloud, showing its contours and surface features as the AF005MNM (Lauro 2019).
A 3D model of a building produced from point cloud data that highlights the architectural elements without color or texture as the Buddha of Bamiyan (Gruen 2004).
Label: ProcessedMesh

dc: description "Relevant for:" Conservation and Enhancement 



—-------------------------------------------------------------------------------------------

F29 Textured 3D Mesh 
URI: https://photogrammetry.altervista.org/items/show/115 
SubClass of: 
D9 Data Object

Scope Note:
The Textured 3D Mesh class refers to a three-dimensional model that has been enhanced with texture mapping, providing detailed surface appearances and color information. This model integrates visual details onto the geometric structure established by the 3D mesh, allowing for realistic representations of artifacts or objects. The texture is applied based on the UV mapping or other texturing techniques, creating a lifelike visual experience suitable for presentation, analysis, and interactive applications.

Examples:

A fully textured 3D model of an archaeological site that reflects the original colors and patterns of the materials used as for the excavation in Gobelklitepe (Polat 2020).
A detailed representation of a historical artifact, showing surface textures and markings based on high-resolution photographs as .
An interactive exhibition display featuring a textured model that enhances the viewer's understanding of the object's form and details as the objects displayed in project BeaVIR (Murtas 2023).
Label: ProcessedTexturedMesh

dc: description "Relevant for:" Conservation and Enhancement 

—-------------------------------------------------------------------------------------------


F30 Acquisition Software 
URI: https://photogrammetry.altervista.org/items/show/116 
SubClass of: 
D14 Software
Scope Note:
The Acquisition Software class refers to the specific software used to perform the acquisition of raw data during a photogrammetric or laser scanning survey. In photogrammetry, it typically refers to the software controlling the camera or capturing images, while for laser scanners or other devices with integrated processing tools, it refers to software exclusively dedicated to data acquisition rather than processing. This software manages the interface between the hardware and the raw data being collected, ensuring that images, point clouds, or other data formats are accurately captured for further processing.
Examples:
The camera control software used during a photogrammetric survey to capture high-resolution images.
Dedicated acquisition software used by a laser scanner to record raw point cloud data without performing any processing steps.
An app that controls a handheld 3D scanner during the acquisition phase of a survey.
The onboard software of a drone camera used for capturing a series of photographs for 3D modeling purposes.
Label: AcquisitionSoftware

dc: description "Relevant for:" Conservation and Enhancement 

—-------------------------------------------------------------------------------------------

F31 Processing Software
URI: https://photogrammetry.altervista.org/items/show/117 
SubClass of: 
D14 Software
Scope Note:
The Processing Software class refers to software specifically used to process raw data into point clouds and densified point clouds during the 3D modeling workflow. This software transforms the data acquired during the acquisition phase (e.g., images from photogrammetry or raw point clouds from laser scanning) and applies algorithms to generate an initial point cloud, followed by densification processes to refine and enrich the dataset. Processing Software is responsible for tasks such as matching, densification, and initial 3D reconstruction steps, ultimately laying the foundation for later stages of modeling. Where possible, expressed with a text string that reports the name of the software and the specific version used. 

Examples:
Software that processes photogrammetric images into an initial sparse point cloud and subsequently applies densification algorithms.
A 3D laser scanner’s companion software that converts raw scan data into a structured point cloud and performs densification.
LiDAR processing software that translates raw light detection and ranging data into a detailed and accurate point cloud.
Applications like Agisoft Metashape, RealityCapture, or Pix4D used to convert raw photogrammetry images into dense point clouds suitable for 3D modeling.
 Zephyr Open Flow 1.3
Label: ProcessingSoftware

dc: description "Relevant for:" teaching and dissemination

—-------------------------------------------------------------------------------------------

F32 Modelling Software
URI: https://photogrammetry.altervista.org/items/show/118 
SubClass of: 
D14 Software
Scope Note:
The Modelling Software class refers to software specifically used to create, modify, and refine 3D models based on processed data, such as point clouds or meshes. Unlike processing software, which applies algorithms for point cloud generation and densification, Modelling Software allows direct manipulation of the 3D model by an operator according to the project's needs. These tasks include editing, reshaping, optimizing the geometry, adjusting scale, and ensuring the model aligns with design specifications or project requirements. The operator has a more hands-on role in this phase, making manual adjustments to the 3D model without intermediary algorithmic processes.
Examples:
Software used to modify 3D meshes, adding or removing details, or reshaping the model.
Programs like Blender, 3ds Max, or Maya, where operators refine models through direct interaction, optimizing them for specific use cases (e.g., rendering, simulation, or 3D printing).
Rhino or SketchUp used for detailed architectural model editing and enhancement.
Label: ModifyngMeshSoftware

dc: description "Relevant for:" Archaeometric analysis 

—-------------------------------------------------------------------------------------------

F33 Acquisition Phase
URI: https://photogrammetry.altervista.org/items/show/119 
SubClass of: 
E29 Design and Procedure
Scope Note:
The Acquisition Phase class refers to the specific set of instructions, protocols, and procedures followed during the acquisition process, as outlined in acquisition manuals or specific acquisition protocols. These guidelines ensure that the collection of raw data (such as photographs, laser scans, or LiDAR readings) follows a standardized and repeatable process, allowing for accurate data capture and the successful reconstruction of 3D models. This class captures all aspects of the acquisition stage, including the positioning of devices, environmental considerations, and calibration steps necessary for consistent data quality across different surveys.
Examples:
Photogrammetry acquisition protocols that specify camera settings, shooting angles, and distances for capturing a complete set of images as FOPPA protocoll (FOPPA).
Laser scanner operating manuals detailing the step-by-step process for capturing modular scans of a structure as Faro Manual (FARO).
LiDAR survey guidelines that outline specific trajectories and scanning methods for archaeological site documentation.
Workflow instructions from photogrammetric or laser scanning handbooks guiding users through the acquisition process as the INCEPTION protocoll (Iadanza 2019).
Label: AcquisitionPhase

dc: description "Relevant for:" Restoration

—-------------------------------------------------------------------------------------------

F34 Processing Phase
URI: https://photogrammetry.altervista.org/items/show/120 
SubClass of: 
E29 Design and Procedure
Scope Note:
The Processing Phase class refers to the set of instructions, protocols, and procedures related to the data processing stage, as described in acquisition manuals or specific acquisition and processing protocols. This phase includes the operations that take place after the acquisition of raw data, such as the generation of point clouds, densification, and the refinement of data through algorithms. These guidelines ensure the transformation of raw data into usable 3D models or datasets, adhering to established methods that guarantee accuracy, consistency, and reproducibility of the processed results.
Examples:
Instructions for generating initial point clouds from photogrammetric images, detailing matching algorithm parameters (FOPPA).
Protocols for processing laser scan data, including steps for point cloud registration and noise filtering (Iadanza 2019).
Guidelines for densifying a point cloud, using specific software configurations (Douglas 2017).
Label: ProcessingPhase

dc: description "Relevant for:" Restoration
—-------------------------------------------------------------------------------------------

F35 Raw Data Carrier
URI: https://photogrammetry.altervista.org/items/show/121 
SubClass of: 
D13 Digital Information Carrier
Scope Note:
The Raw Data Carrier class refers to the physical object that stores digital raw data resulting from an acquisition process, irrespective of the type of acquisition (e.g., photogrammetric, laser scanning, LiDAR, etc.). This class includes devices such as external hard drives, SD cards, USB drives, and any other digital storage media used to preserve and transport unprocessed raw data. The Raw Data Carrier plays a vital role in ensuring that raw data remains accessible for subsequent processing, analysis, and archiving.
Examples:
An external hard drive containing raw LiDAR data from a topographic survey.
An SD card storing raw image data captured during a photogrammetric acquisition.
A USB flash drive with raw laser scan data from an architectural survey.
A cloud storage account holding raw data from a multi-sensor acquisition process.
Label: AcquiredRawDataCarrier

dc: description "Relevant for:" Conservation and Enhancement 

—-------------------------------------------------------------------------------------------

F36 Picture Carrier
URI: https://photogrammetry.altervista.org/items/show/122 
SubClass of: 
F35 Raw Data Carrier
Scope Note:
The Picture Carrier class refers to the physical object that contains digital data, specifically the images captured during a photogrammetric acquisition. This class includes storage devices such as external drives, SD cards, and other digital media that store unprocessed or processed images necessary for the photogrammetric workflow. The Picture Carrier is crucial for the preservation, transportation, and access to the digital image data, ensuring that the photogrammetric survey's raw images remain available for processing and analysis.
Examples:
An SD card storing raw image data from a photogrammetric survey.
An external hard drive containing processed image sets used for 3D reconstruction.
A USB flash drive holding a backup of the photogrammetric images captured during fieldwork.
The server that hosts a cloud storage account that houses the acquired images for future reference and processing.
Label: AcquiredPictureCarrier


—-------------------------------------------------------------------------------------------

F37 Survey Operator 
URI: https://photogrammetry.altervista.org/items/show/123 
SubClass of: 
E39 Actor
Scope Note:
The Survey Operator class refers to the individual responsible for physically performing the survey or acquisition. This person operates the acquisition devices (such as cameras, laser scanners, or LiDAR systems) during the process of data collection. The Survey Operator is in charge of executing the specific survey protocol, ensuring that the equipment functions correctly, and adhering to the instructions or guidelines outlined in the acquisition methodology. This role is crucial for the successful gathering of accurate and high-quality raw data.
Examples:
A photogrammetrist operating a drone-mounted camera for aerial image acquisition of an archaeological site.
A technician using a laser scanner to capture a 3D model of a historical building.
A surveyor manually collecting geospatial data using a handheld GPS device.
An engineer operating a LiDAR system for topographic mapping.
Label: AcquisitionOperator

dc: description "Relevant for:" Archaeometric analysis 


—-------------------------------------------------------------------------------------------

F38 Processing Operator 
URI: https://photogrammetry.altervista.org/items/show/124 
SubClass of: 
E39 Actor
Scope Note:
The Processing Operator class refers to the individual responsible for processing the raw data collected during the acquisition phase. This person uses specific software and algorithms to transform raw data, such as point clouds or images, into more refined outputs like densified point clouds or 3D models. The Processing Operator has to be skilled in utilizing various processing tools to ensure the data is cleaned, aligned, and prepared for subsequent modeling and analysis stages.
Examples:
A technician using photogrammetric software to process raw images and generate a point cloud.
An engineer running processing software on laser scan data to create a densified point cloud.
A 3D specialist refining raw data from a LiDAR survey into a structured, usable format.
An archaeologist processing drone-acquired images to produce orthophotos and digital terrain models.
Label: ProcessingOperator

dc: description "Relevant for:" Archaeometric analysis

—-------------------------------------------------------------------------------------------

F39 Modelling Operator 
URI: https://photogrammetry.altervista.org/items/show/125 
SubClass of: 
E39 Actor
Scope Note:
The Modelling Operator class refers to the individual responsible for the manipulation, modification, and transformation of the 3D model. This person works on refining and adjusting the model based on the specific parameters and requirements of a project, utilizing modeling software to create accurate and detailed 3D representations. The Modelling Operator has to be skilled in various aspects of 3D modeling, such as mesh creation, geometry refinement, and the application of project-specific modifications.

Examples:
A 3D artist refining a photogrammetric model by adjusting the mesh and geometry to create an accurate virtual reconstruction.
An engineer modifying a 3D laser scan model to meet the specific dimensions needed for a structural analysis project.
An archaeologist adjusting the 3D model of an ancient artifact to correct deformations or enhance missing sections.
A heritage specialist applying corrections and detailing to a 3D model of a historical building to prepare it for digital archiving.
Label: ModellingOperator

dc: description "Relevant for:" Conservation and Enhancement 

—-------------------------------------------------------------------------------------------

F40 Eidotype  
URI: https://photogrammetry.altervista.org/items/show/126 
SubClass of: 
E29 Design and Procedure
Scope Note:
The Eydotipe class refers to the sketch or drawing (whether digital or hand-drawn) created by the operator at the time of the survey. This drawing serves to document the general conditions of the surveyed object, including factors such as lighting conditions and the planned trajectory for the acquisition in relation to the object. The Eydotipe is an essential part of the surveying process, providing context and clarity regarding the approach and conditions of the survey.

Examples:
A hand-drawn diagram outlining the positions and angles from which photographs will be taken around an archaeological site.
A digital sketch indicating the lighting setup during the survey of a sculptural piece, noting shadows and reflections.
An annotated drawing that describes the planned trajectory of a laser scanner while capturing data from a complex architectural structure.
A visual representation capturing the environmental conditions at the time of acquisition, such as sunlight direction and weather influences.

Label: AcquisitionEidotype

dc: description "Relevant for:" Archaeometric analysis 

—-------------------------------------------------------------------------------------------

F41 Number of Picture   
URI: https://photogrammetry.altervista.org/items/show/127 
SubClass of: 
E60 Number
Scope Note:
The Number of Picture class refers to the quantitative measurement of the number of individual pictures (F8) that constitute a Picture Set (F7) in a photogrammetric acquisition. This class is used to represent the total count of images captured during a specific acquisition process, which is critical for assessing the completeness and detail of the data collected.
Examples:
A photogrammetric acquisition that consists of 150 images captured from various angles around an archaeological site, where F41 would denote the number "150."
Label: AcquiredNumberOfPicture

dc: description "Relevant for:" Archaeometric analysis 
—-------------------------------------------------------------------------------------------

F42 Place Of Acquisition    
URI: https://photogrammetry.altervista.org/items/show/128 
SubClass of: 
E53 Place
Scope Note:
The Place of Acquisition class refers to the physical space where the acquisition took place, encompassing the location where the acquisition occurred or where the architectural structure that was surveyed is situated. This class is essential for contextualizing the data collected during the acquisition process and provides information on the geographical and cultural relevance of the acquired data. Where possible expressed with a URL on the platform https://www.openstreetmap.org/ 
Examples:
An archaeological site, such as the ruins of an ancient temple, identified as the Place of Acquisition for the photogrammetric survey.
A historic building, like a medieval castle, where the acquisition was performed, serving as the Place of Acquisition.
A landscape feature, such as a valley or a mountain, where the acquisition took place, denoting its significance in geographical studies.
An urban area, like a city square, where multiple structures were surveyed, specified as the Place of Acquisition.
 https://www.openstreetmap.org/way/219582384 
Label: AcquisitionLocation

dc: description "Relevant for:" teaching and dissemination

—-------------------------------------------------------------------------------------------

F43 Survey Date     
URI: https://photogrammetry.altervista.org/items/show/129 
SubClass of: 
E52 Time Span
Scope Note:
The Survey Date class refers to the time period expressed as a specific date when the survey was conducted. This class is crucial for documenting the temporal context of the acquisition process and allows for the establishment of a chronological framework for the collected data. Where possible expressed in XSD 
YYYY indicates the year
MM indicates the month
DD indicates the day
<xs:element name="start" type="xs:date"/>
according to the following indications:
https://www.w3schools.com/xml/schema_dtypes_date.asp

Examples:
The exact date when a photogrammetric survey was performed at a historic site, such as June 15, 2022.
The period during which an archaeological excavation took place, marked with specific survey dates for different phases of the project.
A timeframe noted for monitoring environmental changes, indicating survey dates for repeated assessments at a particular location.
The date assigned to a structural survey conducted on a bridge to evaluate its condition, such as March 1, 2023.
Label: AcquisitionDate

dc: description "Relevant for:" teaching and dissemination

—-------------------------------------------------------------------------------------------

F44 Acquisition Description  
URI: https://photogrammetry.altervista.org/items/show/130 
SubClass of: 
E62 String
Scope Note:
The Acquisition Description class represents a narrative description of the acquisition process. This class allows for the documentation of detailed contextual information regarding the methodologies, conditions, and observations made during the acquisition, enhancing the understanding and interpretation of the collected data.
A description is distinguished from the information already established by other classes as it represents a string where elements not already classified can be annotated and allows a free annotation of information that can help guide the creation of new classes for the ontology.
Examples:
A detailed account of the photogrammetric survey conducted at an archaeological site, including the equipment used, environmental conditions, and specific challenges encountered.
A narrative explaining the steps taken during a laser scanning session, including the trajectory of the device and any notable features of the scanned object.
A description summarizing the purpose and methodology of an acquisition, such as "The survey was conducted to document the structural integrity of the historic building, utilizing a combination of photogrammetry and laser scanning."
A prose description outlining the settings, lighting conditions, and adjustments made during the acquisition process, which may impact the quality of the data collected.
Label: AcquisitionDescription

dc: description "Relevant for:" Archaeometric analysis 

—-------------------------------------------------------------------------------------------

F45 Acquisition Coordinates 
URI: https://photogrammetry.altervista.org/items/show/131 
SubClass of: 
E94 Space Primitive
Scope Note:
The Acquisition Coordinates class refers to the specific spatial coordinates that define the position and orientation of the acquisition device during the data collection process. This class is essential for accurately representing the spatial context of the acquired data, enabling precise alignment and integration with other spatial datasets.
Examples:
The geographic coordinates (latitude, longitude, and altitude) indicating the location where a photogrammetric survey was conducted.
The Cartesian coordinates used to specify the position of a laser scanner during its movement around an object.
A set of coordinates defining the points at which measurements were taken, including their spatial relationship to the object being surveyed.
A description of the coordinate reference system employed during the acquisition, such as WGS84 or a local coordinate system specific to the survey site.
Label: AcquisitionCoordinates 

dc: description "Relevant for:" Conservation and Enhancement 

—-------------------------------------------------------------------------------------------

F46 Matching
URI: https://photogrammetry.altervista.org/items/show/132 
SubClass of: 
F3 Processing
Scope Note:
The Matching class refers to the process of identifying and matching corresponding points or features between multiple images or other forms of raw data. This process is essential in photogrammetry and other surveying methods, as it establishes the spatial relationships between images, allowing the creation of a 3D point cloud. Matching can involve various algorithms and methods to accurately pair points from different perspectives or data sources.
Examples:

The automatic feature matching between pairs of photographs in a photogrammetric workflow to generate an initial sparse point cloud.
The manual identification of common points between overlapping images in cases where automatic matching fails.
The matching of points derived from LiDAR scans to unify multiple scan positions into a coherent 3D point cloud.
Matching points between historical photographs and contemporary images for comparison in archaeological site analysis.
Label: Processing_Matching

dc: description "Relevant for:" Archaeometric analysis

—-------------------------------------------------------------------------------------------


F47 Densification
URI: https://photogrammetry.altervista.org/items/show/133 
SubClass of: 
F3 Processing
Scope Note:
The Densification class refers to the process of enriching the initial sparse point cloud obtained from the Matching phase by adding more data points. This step involves algorithms that interpolate or directly calculate additional points to generate a more detailed and dense representation of the scanned object or scene. Densification is crucial for achieving higher accuracy and detail in the subsequent stages of 3D reconstruction, such as meshing.

Examples:
The densification of a photogrammetric point cloud by increasing the number of points through stereo-matching algorithms.
The use of dense matching techniques to generate a more detailed point cloud in architectural surveys.
The densification of a LiDAR point cloud to increase the resolution and clarity of a 3D terrain model.
Applying densification algorithms in UAV (drone) imagery processing to achieve high-definition surface models.
Label: Processing_Densification

dc: description "Relevant for:" Archaeometric analysis

—-------------------------------------------------------------------------------------------

F48 Densification Method
URI: https://photogrammetry.altervista.org/items/show/134 
SubClass of: 
E29 Design or Procedure

Scope Note:
The Densification Method class refers to the specific procedures, instructions, or algorithms used to carry out the process of densification during the creation of a 3D model. This involves selecting or defining methods that will enrich an initial sparse point cloud by adding more points, which may include techniques based on interpolation, dense matching, or other computational approaches. The densification method directly influences the level of detail and accuracy in the 3D reconstruction process and is essential for achieving a faithful representation of the object or scene being captured.

Examples:
The multi-view stereo (MVS) algorithm for densifying a sparse photogrammetric point cloud.
The algorithm in the software settings for dense matching to increase point density in architectural heritage documentation.
The Semi-Global Matching (SGM) algorithm for densification during the creation of terrain models in UAV mapping.
A specific LiDAR data densification method to capture more detailed features of a landscape.
Label: Processing_DensificationMethod

dc: description "Relevant for:" Restoration

—-------------------------------------------------------------------------------------------

F49  Near Sampling Points Range_SFM Point Seeds
URI: https://photogrammetry.altervista.org/items/show/135 
SubClass of: 
E13 Attribute Assignment
Scope Note:
The Near Sampling Points Range_SFM Point Seeds class refers to the attribute assignment process that involves defining the proximity or range of sampling points used in the densification process, specifically when working with Structure-from-Motion (SfM) point seeds. This class deals with the specification of a radius or tolerance around each seed point in the initial sparse point cloud, within which additional points will be generated or matched during the densification stage. It plays a crucial role in determining the quality and density of the resulting point cloud by controlling how densely points are sampled around the seed points.

Examples:
Setting a sampling radius of 10 pixels around SfM point seeds to guide the densification process in photogrammetry software (Regard 3D).
Specifying the attribute in software that determines the maximum distance within which new points are generated around existing SfM point seeds for terrain modeling (Zephyr 3D) .
Label: DensificationAttribute_NearSamplingPointRange

dc: description "Relevant for:" Archaeometric analysis
—-------------------------------------------------------------------------------------------

F50 Point Cloud Measurement 
URI: https://photogrammetry.altervista.org/items/show/136 
SubClass of: 
S21 Measurement
Scope Note:
The Point Cloud Measurement class refers to the measurement activity that records the quantitative properties of a point cloud, such as the number of points, distribution density, or spatial accuracy. It acts as an intermediary between the F26 Point Cloud and the F51 Point Cloud Number Point, facilitating the process of capturing and evaluating the relevant metrics of the point cloud resulting from 3D acquisition processes. This class is essential for assessing the completeness and precision of the point cloud before further processing or analysis.
Examples:
Measuring the number of points in a point cloud generated by a terrestrial laser scanner.
Assessing the density of points within a 1 cm² area of a point cloud representing an archaeological artifact.
Recording the spatial accuracy of a point cloud based on the standard deviation of point positions.
Measuring the completeness of a point cloud in terms of coverage percentage over a given surface.
Llabe: ProcessedPointCloudMesaurement  

dc: description "Relevant for:" Archaeometric analysis
—-------------------------------------------------------------------------------------------

F51 Point Cloud Number of Point
URI: https://photogrammetry.altervista.org/items/show/137 
SubClass of: 
E54 Dimension
Scope Note:
The Point Cloud Number of Point class refers to the specific dimension that expresses the total number of points composing a non-densified point cloud (F26 Point Cloud). This class quantifies the size of the point cloud in terms of its individual points before the densification process takes place. It is crucial for understanding the initial resolution and completeness of the dataset before additional processing, such as densification or mesh reconstruction.
Examples:
A point cloud generated from a photogrammetry survey containing 500,000 points.
A laser-scanned point cloud consisting of 1.2 million points.
A point cloud obtained from aerial photogrammetry with 750,000 points.
Label: ProcessedPointCloudNumberOfPoint

dc: description "Relevant for:" Archaeometric analysis

—-------------------------------------------------------------------------------------------

F52 Dense Point Cloud Measurement 
URI: https://photogrammetry.altervista.org/items/show/138 
SubClass of: 
S21 Measurement
Scope Note:
The Dense Point Cloud Measurement class refers to the measurement activity specifically related to the dense point cloud (F27 Densified Point Cloud). This class represents the act of assessing and recording dimensions or values that describe the characteristics of a densified point cloud, such as the total number of points. It serves as an intermediary to convey the results of such measurements and link them to the corresponding dense point cloud.

Examples:
-
Label: ProcessedDensePointCloudMeasurement

dc: description "Relevant for:" Archaeometric analysis

—-------------------------------------------------------------------------------------------

F53 Dense Point Cloud Number of Point 
URI: https://photogrammetry.altervista.org/items/show/139 
SubClass of: 
E54 Dimension
Scope Note:
The Dense Point Cloud Number of Point class refers to the specific dimension that indicates the number of points in a densified point cloud (F27 Densified Point Cloud). This class records the total count of points generated after the densification process, offering crucial data about the granularity and density of the final point cloud used for 3D modeling and analysis. Expressed with an integer numeral value.

Examples:

A dense point cloud of a scanned monument containing 15 million points.
32562
Label: ProcessedDensePointCloudNumberOfPoint

dc: description "Relevant for:" teaching and dissemination
—-------------------------------------------------------------------------------------------

F54 Point Cloud Vertex Quality 
URI: https://photogrammetry.altervista.org/items/show/140 
SubClass of: 
E13 Attribute Assignment
Scope Note:
The Point Cloud Vertex Quality class refers to the assignment of quality attributes to individual vertices (points) in a point cloud (F26 Point Cloud). This class records metrics such as positional accuracy, intensity, color information, or other quality-related characteristics that indicate the reliability and precision of the individual vertices in the point cloud dataset.

Examples:
-
Label: ProcessingAttributeVertexQuality

dc: description "Relevant for:" Archaeometric analysis 
—-------------------------------------------------------------------------------------------

F55 Depth Noise Filtering
URI: https://photogrammetry.altervista.org/items/show/141 
SubClass of: E13 Attribute Assignment

Scope Note:
The Depth Noise Filtering class refers to the assignment of depth noise reduction techniques or parameters applied to densified point clouds (F27 Densified Point Cloud). This class captures the process of identifying and filtering out noise, errors, or inaccuracies in the depth values of a point cloud. These filtering operations are particularly necessary in dense datasets where inaccuracies can affect the quality and reliability of subsequent reconstructions.

Examples:
In the densiefied point cloud of AFMNM005 the Depth Noise Filtering is Adaptive feature extraction -AFE-, gradient field estimation -GFE- and further accelerated gradient ascent -FAGA- (Lauro 2019)

Label: DensificationAttributeDepthNoiseFiltering

dc: description "Relevant for:" Archaeometric analysis 
—-------------------------------------------------------------------------------------------

F56 Mesh Reconstruction 
URI: https://photogrammetry.altervista.org/items/show/142 
SubClass of: 
F4 Modelling
Scope Note:
The Mesh Reconstruction class refers to the process of generating a 3D mesh from a densified point cloud (F27 Densified Point Cloud). This class captures the modeling operation where a continuous surface (mesh) is reconstructed, typically using algorithms that define the relationships between individual points within the cloud. This surface representation becomes the foundation for the final 3D model before any texturing is applied, and is crucial for the geometrical definition of the object in digital form.

Examples:
Generating a 3D mesh from a densified point cloud of an archaeological artifact.
Reconstructing the mesh of a building facade from a point cloud acquired through laser scanning in order to create a geometric model for preservation purposes.

Label: Modelling_MeshReconstruction

dc: description "Relevant for:" Archaeometric analysis 
—-------------------------------------------------------------------------------------------

F57 Texturing Mesh 
URI: https://photogrammetry.altervista.org/items/show/143 
SubClass of: 
F4 Modelling
Scope Note:
The Texturing Mesh class refers to the process of applying textures to a 3D mesh in order to enhance its visual appearance. The texture is generally derived from photographs or other 2D image data and is mapped onto the 3D surface to represent the color, material, and finer surface details. This step follows the mesh reconstruction phase and is crucial for adding realism to the 3D model, especially in cultural heritage applications where visual accuracy is important.

Examples:
"Applying high-resolution photographic textures to a 3D mesh of a historic building to accurately reflect its original appearance."
"Mapping surface details onto a 3D model of a statue using images captured from various angles to ensure comprehensive coverage and detail."
"Using UV mapping techniques to accurately position and scale textures on a mesh of an archaeological artifact for virtual exhibition."

Label: Modelling_TexturingMesh

dc: description "Relevant for:" Archaeometric analysis 

—-------------------------------------------------------------------------------------------

F58 Modifying Mesh
URI: https://photogrammetry.altervista.org/items/show/144 
SubClass of: 
F4 Modelling
Scope Note:
The Modifying Mesh class refers to the process of altering or refining a 3D mesh to correct geometrical inaccuracies, simplify the model, or adapt it for specific use cases. This modification can involve smoothing, decimating (reducing the number of polygons), or adjusting the mesh to meet certain criteria, such as improving visual fidelity or optimizing for real-time applications. This step is performed manually or through semi-automated processes and can be part of the workflow in the creation of accurate and efficient 3D models.

Examples:
Modifying the mesh of a historical monument to correct errors introduced during the scanning process.
Simplifying the geometry of a complex 3D model for use in a real-time virtual reality environment.
Label: Modelling_ModifyingTexturedMesh

dc: description "Relevant for:" Conservation and Enhancement 
---------------------------------------------------------------------------

F100 3D Digital Twin 
URI: https://photogrammetry.altervista.org/items/show/145 
SubClass of: 
D9 Data Object
Scope Note:
The 3D Digital Twin class refers to the ultimate 3D model resulting from the complete acquisition and processing workflow. This model may be the outcome of either the F5 Exporting process or F4 Modelling, depending on the workflow followed. At this stage, the model is considered complete and will not undergo any further modifications. It is the final product that represents the culmination of all previous acquisition, processing, and modeling efforts, encapsulating all the geometric and textural information. This final model is typically used for documentation, analysis, visualization, or presentation purposes in various fields such as cultural heritage, architecture, and archaeology. Where possible expressed with a URL linked to the 3D model viewer or the possibility to download it. 

Examples:
The digital twin of the boar jaw preserved at the Okayama archaeological museum and signed as AF005MNM (Lauro 2019).
The digital twin of the excavation section of the Gobelki Tepe site (Polat 2020)
The digital twin of the no longer existing Bayman Buddhas (Gruen 2004).
https://sketchfab.com/3d-models/deltafs-sb-a02-f74fcdba60884fe9aa30106bbb8cfc86 
Label: TridimensionalDigitalTwin

dc: description "Relevant for:" teaching and dissemination
---------------------------------------------------------------------------

F59 Digital Scale  
URI: https://photogrammetry.altervista.org/items/show/146 
SubClass of: 
E54 Dimension
Scope Note:
The Digital Scale class refers to the scale of the 3D Digital Twin (F100), specifically in relation to the actual size of the object being represented. It indicates the proportional relationship between the dimensions of the digital model and the real-world measurements of the original object. This scale can be expressed in various formats, such as 1:1, 1:20, or other ratios, depending on how the 3D model has been created or intended to be used. The Digital Scale is crucial for accurate representation, visualization, and analysis, ensuring that the digital twin correctly reflects the physical dimensions of the object it represents. Where possible expressed according to the following scheme:

Scale of the Surveyed Object:
A: Small object (equal to or smaller than 1 cm)
B: Medium Object (1cm to 30cm)
C: Large Object (from 30 cm upwards)
Q: Open architectural structure
E: Architectural element (part of an architectural structure)
F: Cave or underground structure
G: Landscape element

and expressed according to the measurement of the ideal bounding box in mm
Length, Width followed by Height which will respond to the Geosparql property
 geo:hasSize

https://docs.ogc.org/is/22-047r1/22-047r1.html#_property_geohhassize

and expressed with a ratio between the real scale and the digital scale

Examples:
A digital scale of 1:1 for a final 3D model of a sculpture, indicating that the model is an exact replica of the original size.
A digital scale of 1:50 for an architectural model, showing that the digital representation is 50 times smaller than the actual building.
Label: TridimensionalDigitalTwin_DigitalScale

dc: description "Relevant for:" teaching and dissemination
---------------------------------------------------------------------------

F60 Smoothing Filter   
URI: https://photogrammetry.altervista.org/items/show/147 
SubClass of: 
E13 Attribute Assignment
Scope Note:
The Smoothing Filter class refers to the smoothing filter applied to the 3D Mesh (F28) during its creation process. This filter is used to enhance the quality of the mesh by reducing noise and irregularities, resulting in a more visually appealing and geometrically accurate representation of the 3D object. The application of a smoothing filter is a crucial step in the modeling workflow, as it contributes to the overall aesthetic and functional quality of the final mesh, facilitating better visualization and analysis.
Examples:
A Gaussian smoothing filter applied to a 3D mesh to create a more fluid surface by averaging the vertices of the mesh.
A Laplacian smoothing filter used during the creation of a 3D mesh to reduce sharp edges and create a smoother transition between different surface areas.
Label: ProcessedMeshSmoothingFilter

dc: description "Relevant for:" Archaeometric analysis 
---------------------------------------------------------------------------

F61 Color Balance/Multiband Texture
URI: https://photogrammetry.altervista.org/items/show/148 
SubClass of: 
E13 Attribute Assignment
Scope Note:
The Color Balance/Multiband Texture class refers to the type of texture utilized in the creation of the Textured 3D Mesh (F29). This class encompasses techniques that adjust the color balance and integrate multiple spectral bands to enhance the visual quality of the texture applied to the 3D model. By managing color saturation, brightness, and contrast, this attribute ensures that the texture accurately represents the surface properties of the object, leading to a more realistic and visually appealing 3D representation.

Examples:

A multiband texture that combines data from different spectral bands (such as RGB and infrared) to create a detailed and informative texture for a 3D model of a vegetation area.
A color balance adjustment applied to the texture of a 3D architectural model to ensure that the colors accurately reflect the materials used in the real-world structure.
Label: ProcessedTexturedMeshColorBalance

dc: description "Relevant for:" Archaeometric analysis 
---------------------------------------------------------------------------

F62 Texture Set of 3D Mesh
URI: https://photogrammetry.altervista.org/items/show/149 
SubClass of: 
D9 Data Object
Scope Note:
The Texture Set of 3D Mesh class refers to the collection of textures, which can be either singular or multiple, that are associated with a Textured 3D Mesh (F29). This class encompasses all the visual information applied to the 3D model's surface, which may include different texture maps such as diffuse, specular, normal, and bump maps. The texture set is crucial for enhancing the realism of the 3D model, providing detailed surface characteristics and visual cues that represent the physical properties of the object being modeled. Where possible, this should be expressed with a URL or the exact location of the Repository containing the Texture Set.

Examples:

A texture set consisting of a diffuse map, a normal map, and a specular map used to create a realistic surface appearance for a 3D model of a stone wall.
A collection of multiple textures applied to different parts of a 3D character model, including skin texture, clothing texture, and accessory texture, to achieve a rich and detailed visual representation.
 https://drive.google.com/drive/folders/1l4WFjQnm-6_J9zIJwnIdtkoibkZn3rn7 
Label: ProcessedTexturedMeshTextureSet

dc: description "Relevant for:" teaching and dissemination
---------------------------------------------------------------------------

F63 Number of Texture
URI: https://photogrammetry.altervista.org/items/show/150 
SubClass of: 
E60 Number
Scope Note:
The Number of Texture class refers to the quantity of textures present in a Texture Set of 3D Mesh (F62). This class provides a quantitative measure of the textures utilized in the texturing process of a 3D model, allowing for an understanding of the complexity and detail involved in the visual representation of the model. The number of textures can vary widely depending on the design requirements, intended realism, and specific characteristics of the object being represented.

Examples:

A Texture Set of 3D Mesh consisting of 3 textures, including a diffuse texture for the base color, a normal texture for surface detail, and a specular texture for shininess.
A Texture Set of 3D Mesh that incorporates 5 different textures, each applied to various components of a complex architectural model, such as walls, roofs, windows, and doors.
Label: ProcessedTexturedMeshNumberOfTexture

dc: description "Relevant for:" Conservation and Enhancement 
---------------------------------------------------------------------------

F64 Modelling Description 
URI: https://photogrammetry.altervista.org/items/show/151 
SubClass of: 
E62 String

Scope Note:
The Modelling Description class refers to a prose description of the modelling operations performed on a Textured Mesh (F29) within the context of Modelling (F4). This description provides a narrative account of the changes and modifications made to the 3D model, detailing the techniques, tools, and processes employed during the modelling phase. Such descriptions are essential for documentation purposes, allowing users to understand the adjustments made and the rationale behind them.
A description is distinguished from the information already established by other classes as it represents a string where elements not already classified can be annotated and allows a free annotation of information that can help guide the creation of new classes for the ontology. Where possible, expressed with a text string that describes in detail the modification operations performed on the 3D model before its final export, indicating which elements were eliminated, whether registration and/or alignment operations were performed and what reasons led to such modifications

Examples:

A description detailing how the texture was adjusted to enhance realism by applying a specific smoothing filter and how additional vertices were added to refine the model's geometry.
The string "elimination of the elements of the table and the set and focus on the find " in the context of modeling the 3D model of AF005MNM (Lauro 2019)
"20241107ZETAfsB001c RealityCapture, combination of algorithms, in which Depth Map Fusion and Poisson Surface Reconstruction play a key role. Depth maps are generated from the images and combined to create a continuous and accurate representation of the surface. Poisson Surface Reconstruction is then used to obtain a complete and detailed mesh. deletion of the set and preservation of the detected face of the artifact except for a flap of the set preserved to maintain the metric information and 3D models indicating the position of the cameras at the time of acquisition."

Label: Modelling_ModifyingDescription

dc: description "Relevant for:" teaching and dissemination
---------------------------------------------------------------------------

F65 Modelling Date
URI: https://photogrammetry.altervista.org/items/show/152 
SubClass of: 
E52 Time Span
Scope Note:
The Modelling Date class refers to the specific date when the F58 Modifying Mesh took place. This date is crucial for documenting the timeline of the modelling process, allowing for tracking of changes, revisions, and the overall progression of the 3D model development. Recording the modelling date can aid in understanding the evolution of the model and its context within the broader project timeline.
Examples:
"The F58 Modifyng Mesh of AFMNM005 occurred on 16/03/2019 (Lauro 2019)." 
Label: Modelling_ModifyngTexturedMeshDate

dc: description "Relevant for:" Conservation and Enhancement 
---------------------------------------------------------------------------

F66 Modelling Determination
URI: https://photogrammetry.altervista.org/items/show/153 
SubClass of: 
D7 Digital Machine Event
Scope Note:
The Modelling Determination class refers to the activity of determining which parts of a 3D model should be preserved and which should be eliminated based on project requirements, spatial constraints, and other considerations. This process involves critical decision-making regarding the functionality and aesthetic of the model, ensuring that the final output meets the intended objectives of the project.

Examples:
Assessing which elements of a complex architectural model can be simplified or removed to improve rendering performance.
Deciding which details in a character model are necessary for animation and which can be omitted to optimize the mesh.
Label: Modelling_ModifyingTexturedMeshDetermination

dc: description "Relevant for:" Conservation and Enhancement 
---------------------------------------------------------------------------

F67 Modelling Elimination
URI: https://photogrammetry.altervista.org/items/show/154 
SubClass of: 
D7 Digital Machine Event
Scope Note:
The Modelling Elimination class refers to the actual activity of removing the identified parts from the 3D model as part of the modelling process. This action is taken after the determination phase and is critical for refining the model to meet project specifications and performance requirements.

Examples:
Executing the deletion of unnecessary polygons from a high-resolution model to reduce file size and processing time.
Implementing changes to a 3D asset by removing elements deemed redundant or not relevant to the final output.
Label: Modelling_ModifyingTexturedMeshElimination

dc: description "Relevant for:" Conservation and Enhancement 
---------------------------------------------------------------------------
F68 Digital Twin Physical Carrier
URI: https://photogrammetry.altervista.org/items/show/155 
SubClass of: 
D13 Digital Information Carrier
Scope Note:
The Digital Twin Physical Carrier class refers to the physical storage medium where the Digital Twin (F58) is preserved. This can include various types of physical storage devices, such as external hard drives, SSDs, or any other digital information carriers that ensure the safe storage and accessibility of the Digital Twin for future use.

Examples:
An external hard drive containing the files of a Digital Twin for an architectural project.
The server that host the cloud storage service that stores backups of a Digital Twin for an industrial application.

Label: TridimensionalDigitalTwinCarrier

dc: description "Relevant for:" Conservation and Enhancement 
---------------------------------------------------------------------------

F69 Exporting Description
URI: https://photogrammetry.altervista.org/items/show/156 
SubClass of: 
E62 String
Scope Note:
The Exporting Description class refers to a textual string that contains information and details regarding the operations carried out during the export of the Digital Twin. This description is essential for documenting the export process and can include specifications about formats, settings, and any modifications made during the export.
A description is distinguished from the information already established by other classes as it represents a string where elements not already classified can be annotated and allows a free annotation of information that can help guide the creation of new classes for the ontology.

Examples:

A description detailing the export settings used to generate a 3D model in OBJ format from the Digital Twin.
Notes explaining the conversion process of a Digital Twin from a proprietary format to a standard interchange format for wider accessibility.
Label: ExportingOfTridimensionalDigitalTwinDescription

dc: description "Relevant for:" Archaeometric analysis 

---------------------------------------------------------------------------

F70 Number of Final Destination
URI: https://photogrammetry.altervista.org/items/show/157 
SubClass of: 
E60 Number
Scope Note:
The Number of Final Destination class refers to the quantity of final storage locations for the Digital Twin and all its copies. This metric is important for understanding the distribution and redundancy of the Digital Twin across various storage media, ensuring that the model is preserved in multiple locations for safety and accessibility.

Examples:
The number of backup locations designated for an industrial Digital Twin model.
Count of different cloud storage platforms where copies of a Digital Twin are kept for disaster recovery.
Label: ExportingNumberOfFinalDestination

dc: description "Relevant for:" Archaeometric analysis 

---------------------------------------------------------------------------

F71 Final Use of Digital Twin
URI: https://photogrammetry.altervista.org/items/show/158 
SubClass of: 
D7 Digital Machine Event
Scope Note:
The Final Use of Digital Twin class refers to the final preparations and operations performed on the Digital Twin in accordance with the project's requirements. This class encompasses the generation of all necessary variants of the Digital Twin tailored for specific purposes, ensuring that the final outputs meet the intended application, whether for visualization, simulation, or analysis. Expressed, where possible, according to the following scheme.

1. Teaching and dissemination Generic
1.1 Video Rendering of the 3d Model
1.2 3D Model for AR/VR Projects
1.3 3D Model for Mobile Application
1.4 3D Model for Online Educational Platforms
2. Conservation and Enhancement
2.1 3d Print for Enhancement
2.2 3D Model for interactive projects
2.3 3D Model for Database
3. Archaeometric Analysis
3.1 3D Print for Analysis Preservation
3.2 3D Model for Geographical Information System
3.3 3D Model for Prospectus and Structural Analysis
3.4 3D Model for Computational Fluid Dynamics (CFD) Analysis
4. Restoration Activity
4.1 3D Model for Photogrammetric Comparisons
4.2 3D Model for Precision Molding and Casting
4.3 3D Model for Digital Twins in Restoration Monitoring
4.4 3D Model for Structural Load Analysis


Examples:
Modifying a Digital Twin for use in a virtual reality simulation for a client presentation.
Creating various renditions of a Digital Twin to support different stages of an architectural review process.

Label: Exporting_FinalTridimensionalDigitalTwin
---------------------------------------------------------------------------
F72 3D Model Video Rendering
URI: https://photogrammetry.altervista.org/items/show/159 
SubClass of: 
D9 Data Object
Scope Note:
The 3D Model Video Rendering class refers to the output generated by rendering a 3D model into a video format. This video can be utilized for various purposes, such as presentations, educational demonstrations, or promotional content. The rendering process involves creating a visual representation of the 3D model in motion, showcasing its features, textures, and overall design. Expressed, where possible, with a URL where the video can be viewed

Examples:

A video showcasing the architectural model of a building, rendered to highlight its design elements for a client presentation.
An educational video demonstrating the features of a historical artifact through 3D rendering.
https://youtu.be/AK96WbcQRqE  

Label: Exported3DModelVideoRendering
---------------------------------------------------------------------------

F73 Editing Video
URI: https://photogrammetry.altervista.org/items/show/160 
SubClass of: 
D7 Digital Machine Event
Scope Note:
The Editing Video class refers to the actions performed on the rendered video of the 3D model to modify, enhance, or refine its content. This includes tasks such as cutting, splicing, adding effects, and incorporating audio, all aimed at improving the final presentation quality of the video. Expressed, where possible, with a text string with a detailed description of the editing activities performed on the video project.

Examples:

Cutting segments of the 3D rendering video to create a more concise presentation for a seminar.
Adding background music and transitions to the video of a 3D model for promotional purposes.
Cutting segments of the 3D rendering video to create a more concise presentation for a seminar. Adding background music and transitions to the video of a 3D model for promotional purposes.

Label: Exporting_EditingRenderingVideo
---------------------------------------------------------------------------

F74 Video Editing Software
URI: https://photogrammetry.altervista.org/items/show/161 
SubClass of: 
D14 Software
Scope Note:
The Video Editing Software class refers to the specific applications or programs used to perform the editing operations on the video produced from the 3D model rendering. This software provides tools and features necessary for video manipulation and enhancement, enabling users to create professional-quality videos. Expressed, where possible, with a text string indicating the software and the specific version used

Examples:
Adobe Premiere Pro, used for editing and refining videos of rendered 3D models.
Final Cut Pro, a software application employed in the editing of architectural visualization videos.
Label: Exporting_EditingRenderingVideoSoftware
---------------------------------------------------------------------------

F75 Project Video
URI: https://photogrammetry.altervista.org/items/show/162 
SubClass of: 
D9 Data Object
Scope Note:
The Project Video class refers to the final video product that contains the rendered 3D model, after undergoing editing processes. This video represents the completed work, showcasing the 3D model in a polished format, and is typically used for presentations, marketing, or documentation purposes. Expressed, where possible, with a URL where the video project can be retrieved or alternatively a text string with a description of the location of the original video file. 

Examples:
The final video output showcasing a 3D architectural design, ready for client delivery.
A promotional video that highlights the features of a virtual tour created from a 3D model.
VideoPad Video Editor 1.4.2
Label: ExportedVideo3DRendering

---------------------------------------------------------------------------

F76 3D Model for 3D Print
URI: https://photogrammetry.altervista.org/items/show/163 
SubClass of: 
D9 Data Object
Scope Note:
The 3D Model for 3D Print class refers to a 3D model that has been specifically modified and prepared for 3D printing. This model undergoes adjustments to ensure it meets the necessary specifications and requirements for successful printing, including geometry optimization, scaling, and format compatibility.

Examples:

A 3D architectural model adjusted for printing, with specific wall thickness and support structures included.
A prototype design modified for 3D printing, ensuring all parts are printable without failure.
Label: Exported3DModelForPrinting
---------------------------------------------------------------------------

F77 Printing Digital Twin
URI: https://photogrammetry.altervista.org/items/show/164 
SubClass of: 
E12 Production
Scope Note:
The Printing Digital Twin class refers to the physical action of producing a 3D print of a digital model. This process involves using a 3D printer to convert the digital file of the 3D model into a tangible object, resulting in a physical representation of the digital twin.

Examples:
The operation of a 3D printer producing a scaled model of a historical artifact from a digital file.
The act of 3D printing a prototype based on a digitally designed engineering component.
Label: Exporting_Printing3DModel
---------------------------------------------------------------------------

F78 Material for 3D Printing
URI: https://photogrammetry.altervista.org/items/show/165 
SubClass of: 
E57 Material
Scope Note:
The Material for 3D Printing class refers to the specific type of material selected for use in the 3D printing process. This material is essential for defining the properties and characteristics of the printed object, including its strength, flexibility, and appearance.

Examples:

PLA (Polylactic Acid) used for printing biodegradable models.
ABS (Acrylonitrile Butadiene Styrene) chosen for its durability in engineering applications.
Label: Printed3DModelMaterial
---------------------------------------------------------------------------

F79 Printing Device
URI: https://photogrammetry.altervista.org/items/show/166 
SubClass of: 
E70 Thing
Scope Note:
The Printing Device class refers to the specific model or type of 3D printer utilized for producing the 3D model. This device is responsible for the additive manufacturing process, which builds up the object layer by layer from the material.

Examples:

An FDM (Fused Deposition Modeling) 3D printer used for creating plastic prototypes.
A SLA (Stereolithography) printer employed for high-resolution prints of intricate designs.
Label: 3DPrintingDevice
---------------------------------------------------------------------------

F80 Printed Digital Twin
URI: https://photogrammetry.altervista.org/items/show/167 
SubClass of: 
E18 Physical Thing
Scope Note:
The Printed Digital Twin class refers to the tangible object that results from the 3D printing of a digital twin model. This physical representation retains the features and characteristics of the original digital design and serves various purposes, including prototyping, display, and educational use.

Examples:

A 3D printed model of a historical structure used for educational purposes in a museum.
A prototype of a product that has been physically produced from its digital twin for testing and evaluation.
Label: PrintedTridimensionalDigitalTwin

---------------------------------------------------------------------------

F81 3D Model for G.I.S.
URI: https://photogrammetry.altervista.org/items/show/168 
SubClass of: 
D9 Data Object
Scope Note:
The 3D Model for G.I.S. class refers to a 3D model that has been specifically modified and prepared for implementation within a Geographic Information System (GIS). This model is designed to meet the requirements of GIS applications, including spatial accuracy, scalability, and compatibility with various GIS data formats.

Examples:
A 3D representation of urban infrastructure, adjusted for integration with city planning GIS applications.
A topographical model of a geographical area prepared for environmental analysis within a GIS framework.
Label: ExportedGIS3DModel
---------------------------------------------------------------------------

F82 Reference GIS System
URI: https://photogrammetry.altervista.org/items/show/169 
SubClass of: 
D9 Data Object
Scope Note:
The Reference GIS System class refers to the specific Geographic Information System in which the 3D model will be inserted. This system serves as the platform for managing, analyzing, and visualizing spatial data, including the 3D model.

Examples:

A municipal GIS used for urban planning and zoning, where the 3D model represents building structures.
A conservation GIS employed in environmental management, integrating 3D models of natural landscapes.
Label: GISSystem
---------------------------------------------------------------------------

F83 GIS Software
URI: https://photogrammetry.altervista.org/items/show/170 
SubClass of: 
D14 Software
Scope Note:
The GIS Software class refers to the specific software application used for managing and analyzing geographical information. This software supports the functionality necessary to incorporate 3D models into the GIS, enabling spatial analysis, visualization, and data manipulation.

Examples:

ArcGIS, a popular GIS software for mapping and spatial analysis, supporting the integration of 3D models.
QGIS, an open-source GIS application that allows users to work with 3D representations of spatial data.

Label: GISSoftware
---------------------------------------------------------------------------
F84 3D Model for Prospectus
URI: https://photogrammetry.altervista.org/items/show/171 
SubClass of: 
D9 Data Object
Scope Note:
The 3D Model for Prospectus class refers to a 3D model that has been specifically modified and prepared to derive plans, elevations, orthophotos, and other information regarding sections, topographical features, and architectural elements. This model serves as a foundational tool for generating accurate representations and documentation related to the spatial attributes of a structure or area.

Examples:

A modified 3D model of a building used to create architectural plans and sections.
A terrain model used to generate topographic maps and orthophotos for environmental studies.
Label: Exported3DModelForProspectus
---------------------------------------------------------------------------
F85 CAD Analysis
URI: https://photogrammetry.altervista.org/items/show/172 
SubClass of: 
D7 Digital Machine Event

Scope Note:
The CAD Analysis class refers to the actions performed to extract plans, elevations, orthophotos, and other information regarding sections, topographical features, and architectural data from the 3D model. This process involves various analytical and computational techniques to ensure the accuracy and utility of the generated outputs.

Examples:

Using CAD software to create detailed floor plans and architectural drawings from a 3D model.
Analyzing a 3D terrain model to produce accurate orthophotos for cartographic purposes.
Label: Exporting_CADAnalysis
---------------------------------------------------------------------------
F86 Software CAD
URI: https://photogrammetry.altervista.org/items/show/173 
SubClass of: 
D14 Software
Scope Note:
The Software CAD class refers to specific software applications used for Computer-Aided Design (CAD). This software supports the creation, modification, and analysis of 3D models to derive architectural and topographical information, facilitating detailed design and engineering processes.

Examples:
AutoCAD
Revit
Label: CADSoftware
---------------------------------------------------------------------------
F87 3D Model Prospectus
URI: https://photogrammetry.altervista.org/items/show/174 
SubClass of: 
D9 Data Object

Scope Note:
The 3D Model Prospectus class refers to the output products such as plans, orthophotos, and any type of information generated from the CAD analysis performed on the 3D model. This class encompasses the documentation and visual representations that emerge from the analytical processes.

Examples:
A set of architectural elevations and floor plans derived from a 3D building model.
An orthophoto map created from a topographical model after CAD analysis.
Label: ExportedCAD3DModelProspectus

---------------------------------------------------------------------------

F88 Archaeometric 3D Model
URI: https://photogrammetry.altervista.org/items/show/175 
SubClass of: 
D9 Data Object

Scope Note:	
The Archaeometric 3D Model class refers to a 3D model that has been specifically prepared for archaeometric analysis, as well as for general analysis of the object's surface characteristics. This type of model is intended for detailed examination, allowing researchers to assess material properties, deterioration, and other relevant factors.

Examples:

A 3D scan of an ancient artifact prepared for materials analysis.
A detailed model of a historic building surface analyzed for degradation patterns.
Label: ExportedArchaeometricTridimensionalDigitalTwin
---------------------------------------------------------------------------

F89 Project Analysis
URI: https://photogrammetry.altervista.org/items/show/176 
SubClass of: 
D7 Digital Machine Event

Scope Note:
The Project Analysis class refers to the digital operations performed to analyze the 3D model and study its surface in detail. This analysis may involve various techniques and methodologies aimed at revealing insights about the object's structure, condition, and materials.

Examples:

Conducting a surface analysis of a 3D archaeological model to identify wear patterns.
Performing a digital evaluation of a historical artifact to assess its preservation status.
Label: Exporting_ArchaeometricAnalysis
---------------------------------------------------------------------------
F90 Data Log Analysis
URI: https://photogrammetry.altervista.org/items/show/177 
SubClass of: 
D9 Data Object

Scope Note:
The Data Log Analysis class refers to a text file that contains information derived from the analysis or produced directly from the digital analysis processes. This file serves as a record of findings and observations, enabling further investigation and documentation.

Examples:

A CSV file detailing measurements and observations from a 3D surface analysis.
A log of the parameters used in digital analysis processes, including any findings related to the object being studied.
Label: ExportedArchaeometricDataLogAnalysis
---------------------------------------------------------------------------

F91 Model for Interactive
URI: https://photogrammetry.altervista.org/items/show/178 
SubClass of: 
D9 Data Object

Scope Note:
The Model for Interactive class refers to a 3D model that has been prepared and modified for display in an interactive digital presentation. This model is designed to enhance user engagement and provide an immersive experience in exploring the model's features and characteristics.

Examples:

A 3D reconstruction of an archaeological site created for interactive educational software.
A digitally enhanced model of a historical building intended for virtual tours.

Label:  ExportedTridimensionalDigitalTwinForInteractive
---------------------------------------------------------------------------

F92 Interactive Project Implementation
URI: https://photogrammetry.altervista.org/items/show/179 
SubClass of: 
D7 Digital Machine Event

Scope Note:
The Interactive Project Implementation class refers to the process of integrating the Model for Interactive (F91) into a specific interactive visualization project. This activity encompasses the technical steps required to ensure that the model functions effectively within the interactive environment.

Examples:

Incorporating a 3D model into a virtual reality application for educational purposes.
Setting up an interactive display that allows users to manipulate and explore a historical model.
Label: Exporting_InteractiveProjectImplementation
---------------------------------------------------------------------------

F93 Interactive Software
URI: https://photogrammetry.altervista.org/items/show/180 
SubClass of: 
D14 Software

Scope Note:
The Interactive Software class refers to the software utilized to create the interactive project, such as Unity or other platforms designed for developing interactive visual experiences. This software supports the creation and integration of 3D models into engaging formats.

Examples:

Unity.
Unreal Engine.
Label: InteractiveProjectSoftware

---------------------------------------------------------------------------
F94 3D Model for Database
URI: https://photogrammetry.altervista.org/items/show/181 
SubClass of: 
D9 Data Object

Scope Note:
The 3D Model for Database class refers to a 3D model that has been modified and prepared for upload to a project database. This model is structured to meet the requirements of database management systems and is intended for efficient storage, retrieval, and management within a digital environment.

Examples:

A 3D representation of an archaeological artifact prepared for storage in a digital archive.
A model of a historical site optimized for inclusion in a geographic database.
Label: Exported3DModelForDatabase
---------------------------------------------------------------------------

F95 Database Project Implementation
URI: https://photogrammetry.altervista.org/items/show/182 
SubClass of: 
D7 Digital Machine Event

Scope Note:
The Database Project Implementation class refers to the activity of uploading the 3D model (F94) to a specific database. This process involves the technical steps necessary to ensure the model is correctly integrated and accessible within the database framework.

Examples:

The process of importing a 3D model into a cultural heritage database.
Uploading a digital representation of a building to a municipal database for urban planning.
Label: Exporting_DatabaseImplementation
---------------------------------------------------------------------------
F96 Database Architecture
URI: https://photogrammetry.altervista.org/items/show/183 
SubClass of: 
D14 Software

Scope Note:
The Database Architecture class refers to the software and/or specific architecture utilized in the database where the 3D model (F94) has been uploaded. This may include details about the database management system, data structure, and design principles that facilitate effective data storage and access.

Examples:

SQL-based databases used for managing 3D models in cultural heritage projects as Omeka-s.
Wikibase 
Label: DatabaseArchitectureSoftware
---------------------------------------------------------------------------

F97 AR 3D Model
URI: https://photogrammetry.altervista.org/items/show/184 
SubClass of: 
D9 Data Object

Scope Note:
The AR 3D Model class refers to a 3D model that has been modified and prepared for implementation in an Augmented Reality (AR) or Mixed Reality (MR) project. This model is designed to interact with real-world environments and enhance user experiences through digital overlays. Expressed, where possible, with a URL of the viewer or download link of the model used.

Examples:

A 3D reconstruction of a historical site intended for an AR application.
A virtual artifact designed to be viewed in a mixed reality setting.
https://sketchfab.com/3d-models/yaioi-boar-jaw-3136f87dde21439c953f62d2e19293d4 
  
Label: ExportedAR3DModel
---------------------------------------------------------------------------
F98 AR/MR Project Implementation
URI: https://photogrammetry.altervista.org/items/show/185 
SubClass of: 
D7 Digital Machine Event

Scope Note:
The AR/MR Project Implementation class refers to the process of integrating the AR 3D model (F97) into a specific Augmented Reality or Mixed Reality project. This includes the technical steps required to ensure the model functions properly within the AR/MR environment. Expressed, where possible, with a text string with a detailed description of the activity and operations performed.

Examples:

Loading a 3D model into an AR application for mobile devices.
Integrating a virtual object into a mixed reality experience for educational purposes.
model exported as FBX and uploaded in Unity project 
Label: Exporting_AR-MRProjectImplementation

---------------------------------------------------------------------------
F99 AR Software Modelling
URI: https://photogrammetry.altervista.org/items/show/186 
SubClass of: 
D14 Software

Scope Note:
The AR Software Modelling class refers to the software used in the Augmented Reality or Mixed Reality project where the AR 3D model (F97) has been loaded. This software facilitates the creation and deployment of interactive AR experiences. Expressed, where possible, with a text string indicating the software and the specific version adopted

Examples:

Unity.
Vuforia.

Label: AR-MRImplementationSoftware
---------------------------------------------------------------------------
F101: Survey Phase
URI: https://photogrammetry.altervista.org/items/show/187 
Subclass of: 
E29 Design and Procedure

Scope Note:
The Survey Phase refers to a stage within the acquisition process, which can be divided into various moments such as acquisition, processing, and analysis. Each phase within the survey process addresses a specific task or set of tasks that contribute to the overall objective of collecting spatial, visual, or other relevant data about an object or environment. A Survey Phase may encompass the preparation of equipment, calibration, field operations, and initial data checks, ensuring that the collected data adheres to predefined technical standards. The phases may vary depending on the project’s design and procedural requirements, contributing to the systematic and reproducible execution of the survey. Where possible express the Survey Phase identifier use the model Date of Survey+SurveyPhase+Path Used For the Survey+Scale of the surveyed object+identifying number of the object where it is considered that:
Survey Phase:
ALFA: First Survey Coincident with the discovery or first survey project
BETA: First Survey on a classified object for more than 2 years
GAMMA: Second survey on an already surveyed object
DELTA: Third survey an already surveyed object
EPSILON: over the third survey of an already surveyed object
ZETA: Survey of a 3d print of surveyed object
ETA: Virtual survey of a 3d survey in virtual context

Path Used for the survey:
fs: freehand spiral
lf: linear freehand
ad: aerial wireless
vl: vertical or with drone or with rod
sb: spiral with rotating base
 el: easel linear
 sm: structured mixed
mu: mixed unstructured
rm: rotating base microscope
rb: rotating base fixed instrument

Scale of the Surveyed Object:
A: Small object (equal to or smaller than 1 cm)
B: Medium Object (1cm to 30cm)
C: Large Object (from 30 cm upwards)
Q: Open architectural structure
E: Architectural element (part of an architectural structure)
F: Cave or underground structure
G: Landscape element

object identification number
Progressive number in order of acquisition starting from 001 up to 999.


Examples:
The Survey Phase involved an initial site walk-through and preparation, followed by the actual data acquisition using a terrestrial laser scanner.
20190309BETAfsB001 

Label: SurveyPhase

dc: description "Relevant for:" teaching and dissemination

—-------------------------------------------------------------------------
F102: 3D Digital Asset
URI: https://photogrammetry.altervista.org/items/show/188 
Subclass of:
	D9 Data Object
Scope Note:
	The 3D Digital Asset class refers to a broad category of digital objects that represent three-dimensional entities. This class includes various specific types of 3D models, such as F100 3D Digital Twin, F28 3D Mesh, F29 Textured 3D Mesh, F76 3D Model for 3D Print, F81 3D Model for GIS, F84 3D Model for Prospectuses, F88 Archaeometric 3D Model, F91 3D Model for Interactive, F94 3D Model for Database, and F97 AR 3D Model.
A 3D Digital Asset is defined by its ability to represent surfaces, volumes, and textures of objects in a coherent and structured manner, typically through vertices, edges, faces, or other geometric components (such as meshes) that form the basis of digital three-dimensional models. These assets are often the result of post-processing stages that follow raw data collection, such as point clouds, and include enhanced visual and structural information like textures, color mapping, or other metadata related to the object's properties or context.
It is important to note that Point Clouds (as represented by F26 Point Cloud and F27 Dense Point Cloud) are excluded from this class. Point clouds are raw collections of data points in a three-dimensional space that define the surface of an object or scene without structured geometric relationships (e.g., faces, volumes). While point clouds represent a step in the acquisition process, they lack the interconnected geometry and texturing that are characteristic of 3D Digital Assets. A 3D Digital Asset, on the other hand, contains processed, refined, and sometimes enriched information, making it suitable for various applications, including simulations, renderings, interactive platforms, and analysis tools.
Examples:
A 3D Digital Asset was created as a Textured 3D Mesh (F29) of a historical monument, used for digital documentation and preservation.
The 3D Digital Twin (F100) of an industrial component was generated for predictive maintenance and simulations.
A 3D Model for GIS (F81) was developed to integrate geographical and cultural heritage data into a spatial analysis platform.
Label: TridimensionalDigitalAsset
—------------------------------------------------------------------------
F103: Calibration (Camera Calibration)
URI: https://photogrammetry.altervista.org/items/show/189 
Subclass of:
F46 Matching
Scope Note:
The F103 Calibration class represents the camera calibration process used during photogrammetric data acquisition. Camera calibration is a crucial step in the photogrammetric workflow to ensure that the captured images are accurately mapped to a three-dimensional coordinate system and to correct any intrinsic and extrinsic optical distortions in the camera. The class describes the calibration parameters related to the camera, including focal length, principal point, radial and tangential distortion coefficients, and other optical properties.
Calibration aims to enhance the quality and accuracy of the 3D models generated through photogrammetry by minimizing systematic errors that may affect the final result. This process can be carried out before or during the image acquisition phase and typically involves a known set of reference points or calibration grids to determine the camera’s geometric properties.
F103 is part of the broader process of matching and optimizing data in the context of digital surveying, represented by F46 Matching, of which F103 is a subclass. Calibration ensures accurate correspondence between image data and the physical world, facilitating the subsequent processing and 3D modeling phases.

Examples:
A camera calibration (F103) was performed prior to a photogrammetric survey to correct for optical lens distortion and improve the accuracy of the generated 3D model.
During image acquisition for an archaeological project, camera calibration (F103) enabled the collection of optimized data for subsequent 3D model creation.
The calibration (F103) was applied to correctly align multiple images in photogrammetry software, ensuring an accurate reconstruction of the 3D scene.
Label: Processing_Matching_Calibration

dc: description "Relevant for:" Archaeometric analysis 
—-----------------------------------------------------------------------
F104: Registration (Fusion of Multiple Point Clouds or 3D Models)
URI: https://photogrammetry.altervista.org/items/show/190 
Subclass of:

F27 Densified Cloud Point

Scope Note:
The F104 Registration class refers to the accomplished process of aligning and merging multiple point clouds into a single unified model. This class specifically deals with point clouds resulting from the registration process, known as densified point clouds. These are highly detailed datasets generated through the alignment of overlapping point clouds, typically collected from different viewpoints, platforms or scanning techniques. The registration process ensures that multiple datasets are accurately aligned within a common coordinate system and that the resulting densified point cloud forms a more complete and precise representation of the object or scene.

The resulting point cloud (F104) is the result of key activities which in this process include matching features or corresponding points between point clouds, applying algorithms to minimize alignment errors, and optimizing the model for consistency and precision. Densified point clouds are critical in photogrammetry and 3D reconstruction workflows, especially for complex objects or large-scale environments that require the integration of multiple scans. The course captures both manual and automated registration approaches, with a focus on methods used to create a unified, high-resolution point cloud from separate initial data sources.


Examples:

The densified point cloud (F104) generated by registering multiple scans of a historical building from different angles allowed for the creation of a high-resolution 3D model for conservation documentation.
During the survey of a large archaeological site, multiple point clouds from drone and ground-based LiDAR scans were registered (F104) and merged to form a unified model representing the entire site in high detail.
Automated registration (F104) was used to combine aerial LiDAR data and ground-based photogrammetry scans of a forested area, resulting in a dense point cloud model for environmental analysis.
The registration (F104) of point clouds captured from different structural elements of a bridge allowed for the creation of a densified model used for structural integrity analysis.

Label: ProcessedDensifiedPointCloudRegistration

dc: description "Relevant for:" Conservation and Enhancement 


—--------------------------------------------------------------------------- 
 
F105: Interrogation Tools (Digital Instruments for Measuring Cloud Points or 3D Models)
URI: https://photogrammetry.altervista.org/items/show/191 
Subclass of:
D14 Software

Scope Note:
The F105 Interrogation Tools class refers to software-based tools and algorithms used for measuring, analyzing, and manipulating Cloud Points or 3D Models in a digital environment. This class includes a variety of specialized software solutions, plugins, or standalone programs that allow users to perform precise measurements on 3D digital representations, such as calculating distances, volumes, surface areas, and other geometrical or spatial properties.
These interrogation tools are integral to post-processing and analysis in photogrammetry and 3D modeling workflows. They enable deeper examination and understanding of 3D data by applying advanced algorithms or providing user-friendly interfaces to visualize and interact with the data. Examples of functions provided by F105 Interrogation Tools include surface analysis, point cloud comparison, texture mapping, and deformation tracking.
By being a subclass of D14 Software, F105 reflects that the tools in this class are entirely software-based digital devices rather than hardware, and are designed to process and interact with digital models or datasets within a virtual environment.

Examples:

Software-based tools (F105) were applied to a dense point cloud to measure the volume of an archaeological excavation site.
A curvature analysis tool (F105) was used to evaluate the surface smoothness of a digital 3D model of an ancient sculpture.
A point cloud comparison tool (F105) was employed to assess differences between two scans of a building facade taken months apart to monitor structural changes.
Texture mapping interrogation software (F105) was utilized to assess how accurately textures were applied to a 3D model for virtual exhibition purposes.

Label: InterrogationToolsSoftware

dc: description "Relevant for:" Restoration



Y1: is acquired object of
Y2: had pictures input
Y3: has Type Of Acquisition
Y4: has dominant geometry type
Y5: has scale type
Y6: used trajectory
Y7: has method of acquisition
Y8: happened on acquisition device
Y9: has acquisition device type
Y10: has created raw data
Y11: used acquisition software
Y12: was continued by Processing Phase
Y13: used Acquisition Instruction
Y14: stores acquisition Picture
Y15: is composed of picture
Y16: has number of picture
Y17: has acquisition operator
Y18: has place of acquisition
Y19: has date of acquisition
Y20: has acquisition description
Y21: has coordinates of acquisition
Y22: had acquisition input
Y23: has type of matching
Y24: happened on processing device
Y25: Processing is composed of
Y26: used processing software
Y27: has method of densification
Y28: has type of densification
Y29: has matching input
Y30: has created point cloud
Y31: has created densified point cloud
Y32: has method of matching
Y33: has observed number of points
Y34: was measured in number of points
Y35: has vertex quality assignment
Y36: has Depth Noise Filtering
Y37: has observed number of points (for dense point clouds)
Y38: was measured in number of points (for dense point clouds)
Y39: has Sampling Points Range
Y40: has processing operator
Y41: used Phase Instruction
Y42: was continued by Modelling phase
Y43: has type of texturing
Y44: has type of reconstruction
Y45: point cloud input
Y46: has created 3D Mesh
Y47: has method of reconstruction
Y48: has method of texturing
Y49: has created Digital Twin
Y50: happened on modelling device
Y51: Modelling is composed of
Y52: 3D mesh input
Y53: Textured 3D mesh input
Y54: has created textured 3D mesh
Y55: has digital scale
Y56: has smoothing filter
Y57: has color balance/multiband
Y58: has number of texture
Y59: is texture set of
Y60: has modelling description
Y61: used modelling software
Y62: has modelling operator
Y63: has date of acquisition
Y65: Modelling is influenced by
Y66: is Digital Twin physical carrier
Y67: was continued by Exporting phase
Y68: has Textured 3D Model as input
Y69: has Digital Twin as output
Y70: Final Use of 3D Model consists of
Y71: has number of final destination
Y72: had final use output
Y73: had rendering as input
Y74: use video editing software
Y75: had Video output
Y76: printing based on
Y77: has printed physical digital twin
Y78: used specific printing machine
Y79: consists of printing material
Y80: is in GIS
Y81: used GIS software
Y82: had model prospectuses for CAD as input
Y83: used CAD software
Y84: had prospectus output
Y85: had archaeometric input
Y86: had data log analysis output
Y87: had 3D model interactive as input
Y88: used interactive software
Y89: had 3D model for database as input
Y90: used database software/architecture
Y91: had 3D model for AR as input
Y92: used AR/MR software
Y93: was continued by subsequent phase
Y94: has observed number of points
Y95: was measured in number of points
References
Ontology and Thesaury References
Manual of Acquisition


—------------------------------------------------------------------------

Y1: is acquired object of 
URI: https://photogrammetry.altervista.org/items/show/192 
SubProperties of: L1 digitized

Domain: F2 Acquisition
Range: F1 Survey Object

Scope Note:
This property refers to the specific survey object (F1) that was the subject of the acquisition process (F2). It indicates the object being digitized or acquired during a particular survey or documentation effort.

Examples:
 
Label: is_acquired_of

—--------------------------
Y1: is acquired object of
Inverse: Y1-Inverse: is object acquired by
Label: "is object acquired by"
Domain: F1 Survey Object
Range: F2 Acquisition

—------------------------------------------------------------------------

Y2: had pictures input
URI: https://photogrammetry.altervista.org/items/show/193 
SubProperties of: L10 had input

Domain: F2 Acquisition
Range: F7 Picture Set

Scope Note:
This property refers to the set of pictures (F7) that were used as input during an acquisition event (F2). It connects the acquisition process to the photographic data that was collected or processed.

Examples:
 

Label: had_pictures_input
—--------------------------
Y2: had pictures input
Inverse: Y2-Inverse: is input picture set for
Label: "is input picture set for"
Domain: F7 Picture Set
Range: F2 Acquisition

—------------------------------------------------------------------------

Y3: has Type Of Acquisition
URI: https://photogrammetry.altervista.org/items/show/194 
SubProperties of: P2 has type

Domain: F12 Acquisition Trajectory
Range: F17 Acquisition Trajectory Type

Scope Note:
This property identifies the type of trajectory used during an acquisition event (F12). It specifies the method or approach taken to move through space and acquire data, such as linear, circular, or other types of trajectories.

Examples:
 
Label: has_type_of_acquisition
—--------------------------
Y3: has Type Of Acquisition
Inverse: Y3-Inverse: is acquisition type of
Label: "is acquisition type of"
Domain: F17 Acquisition Trajectory Type
Range: F12 Acquisition Trajectory
—------------------------------------------------------------------------

Y4: has dominant geometry type
URI: https://photogrammetry.altervista.org/items/show/195 
SubProperties of: P2 has type

Domain: F13 Acquisition Method
Range: F18 Geometry Type

Scope Note:
This property describes the dominant geometry type (F18) captured during an acquisition method (F13). It indicates whether the acquisition primarily involved points, lines, surfaces, or volumes.

Examples:
 
Label: has_dominant_geometry_type
—--------------------------
Y4: has dominant geometry type
Inverse: Y4-Inverse: is dominant geometry type of
Label: "is dominant geometry type of"
Domain: F18 Geometry Type
Range: F13 Acquisition Method

—------------------------------------------------------------------------

Y5: has scale type
URI: https://photogrammetry.altervista.org/items/show/196 
SubProperties of: P2 has type

Domain: F13 Acquisition Method
Range: F19 Scale Type

Scope Note:
This property refers to the scale type (F19) associated with the acquisition method (F13). It defines whether the acquisition was performed on a small, medium, or large scale, according to the object and purpose of the survey.

Examples:

 
Label: has_scale_type
—--------------------------
Y5: has scale type
Inverse: Y5-Inverse: is scale type of
Label: "is scale type of"
Domain: F19 Scale Type
Range: F13 Acquisition Method

—------------------------------------------------------------------------

Y6: used trajectory
URI: https://photogrammetry.altervista.org/items/show/197 
SubProperties of: P33 used specific technique

Domain: F2 Acquisition
Range: F12 Acquisition Trajectory

Scope Note:
This property describes the specific trajectory (F12) used during the acquisition event (F2). It denotes the path or movement employed to capture data.

Examples:
 
Label: used_trajectory
—--------------------------
Y6: used trajectory
Inverse: Y6-Inverse: is trajectory used by
Label: "is trajectory used by"
Domain: F12 Acquisition Trajectory
Range: F2 Acquisition

—------------------------------------------------------------------------

Y7: has method of acquisition
URI: https://photogrammetry.altervista.org/items/show/198 
SubProperties of: P33 used specific technique

Domain: F2 Acquisition
Range: F13 Acquisition Method

Scope Note:
This property refers to the method (F13) utilized in an acquisition process (F2). It identifies the particular technique or procedure, such as photogrammetry or LiDAR scanning, used to acquire data.

Examples:
 
Label:  has_method_of_acquisition
—--------------------------
Y7: has method of acquisition
Inverse: Y7-Inverse: is acquisition method of
Label: "is acquisition method of"
Domain: F13 Acquisition Method
Range: F2 Acquisition

—------------------------------------------------------------------------

Y8: happened on acquisition device
URI: https://photogrammetry.altervista.org/items/show/199 
SubProperties of: L12 happened on device

Domain: F2 Acquisition
Range: F9 Acquisition Device

Scope Note:
This property refers to the acquisition device (F9) on which the acquisition process (F2) occurred. It links the acquisition event to the specific piece of hardware or equipment used.

Examples:
 

Label: happened_on_acquisition_device
—--------------------------
Y8: happened on acquisition device
Inverse: Y8-Inverse: is device used for acquisition
Label: "is device used for acquisition"
Domain: F9 Acquisition Device
Range: F2 Acquisition

—------------------------------------------------------------------------

Y9: has acquisition device type
URI: https://photogrammetry.altervista.org/items/show/200 
SubProperties of: L17 measured thing of type

Domain: F2 Acquisition
Range: F20 Acquisition Device Type

Scope Note:
This property specifies the type of acquisition device (F20) used during the acquisition process (F2). It identifies the general category or kind of device employed, such as a camera, scanner, or drone.

Examples:
 
Label: has_acquisition_device_type
—--------------------------
Y9: has acquisition device type
Inverse: Y9-Inverse: is acquisition device type of
Label: "is acquisition device type of"
Domain: F20 Acquisition Device Type
Range: F2 Acquisition
—------------------------------------------------------------------------

Y10: has created raw data
URI: https://photogrammetry.altervista.org/items/show/201 
SubProperties of: L11 has output

Domain: F2 Acquisition
Range: F6 Acquisition Raw Data

Scope Note:
This property refers to the raw data (F6) generated as a result of the acquisition event (F2). It connects the acquisition process to the unprocessed, primary data produced during the survey.

Examples:

The relation between the point cloud data generated and the  laser scanning session.
The relation between the raw images captured and the photogrammetric survey of a building façade.

Label: has_created_raw_data
—--------------------------
Y10: has created raw data
Inverse: Y10-Inverse: is raw data created by
Label: "is raw data created by"
Domain: F6 Acquisition Raw Data
Range: F2 Acquisition
—------------------------------------------------------------------------

Y11: used acquisition software
URI: https://photogrammetry.altervista.org/items/show/202 
SubProperties of: L23 used software or firmware

Domain: F2 Acquisition
Range: F30 Acquisition Software

Scope Note:
This property refers to the specific software (F30) used during the acquisition event (F2). It identifies the software that controlled the data capture or processed the initial acquisition.

Examples:
-

Label: used_acquisition_software
—--------------------------
Y11: used acquisition software
Inverse: Y11-Inverse: is software used for acquisition
Label: "is software used for acquisition"
Domain: F30 Acquisition Software
Range: F2 Acquisition

—------------------------------------------------------------------------

Y12: was continued by Processing Phase

This property is redundant and can be replaced by the superproperty 
-Y93 was continued by subsequent phase-

SubProperties of: P134i was continued by

Domain: F2 Acquisition
Range: F3 Processing

Scope Note:
This property describes how the acquisition event (F2) was followed by a processing phase (F3). It links the data acquisition process to the subsequent phase where raw data is processed and refined.

Examples: 
 
Label: was_continued_by_processing_phase

—------------------------------------------------------------------------

Y13: used Acquisition Instruction
URI: https://photogrammetry.altervista.org/items/show/204 
Subproperty of: P33 used specific technique

Domain: F2 Acquisition
Range: F33 Acquisition Phase

Scope Note:
This property links the acquisition event (F2) to the specific acquisition instructions or procedures (F33) that were used to guide the process. These instructions may define steps, settings, or approaches used during the acquisition phase.

Examples:

 
Label: used_acquisition_instruction
—--------------------------
Y13: used Acquisition Instruction
Inverse: Y13-Inverse: is instruction used by acquisition
Label: "is instruction used by acquisition"
Domain: F33 Acquisition Phase
Range: F2 Acquisition

—------------------------------------------------------------------------

Y14: stores acquisition Picture
URI: https://photogrammetry.altervista.org/items/show/205 
Subproperty of: L19 stores

Domain: F35 Raw Data Carrier
Range: F8 Picture

Scope Note:
This property connects a raw data carrier (F35) to the pictures (F8) it stores. It identifies the images that were collected during the acquisition process and are saved on a specific storage device or medium.

Examples:

 

Label: stores_acquisition_picture
—--------------------------
Y14: stores acquisition Picture
Inverse: Y14-Inverse: is acquisition picture stored in
Label: "is acquisition picture stored in"
Domain: F8 Picture
Range: F35 Raw Data Carrier
—------------------------------------------------------------------------

Y15: is composed of picture  
URI: https://photogrammetry.altervista.org/items/show/206 
Subproperty of: P106 is composed of

Domain: F7 Picture Set
Range: F8 Picture

Scope Note:
This property indicates that a picture set (F7) is composed of individual pictures (F8). It defines the relationship between the collection of images used for acquisition and the individual pictures that constitute the set.

Examples:

 
Label:  is_composed_of_picture
—--------------------------
Y15: is composed of picture
Inverse: Y15-Inverse: is picture part of
Label: "is picture part of"
Domain: F8 Picture
Range: F7 Picture Set

—------------------------------------------------------------------------

Y16: has number of picture
URI: https://photogrammetry.altervista.org/items/show/207 
Not a subproperty of any other property

Domain: F7 Picture Set
Range: F41 Number of Picture

Scope Note:
This property describes the number of individual pictures contained in a picture set (F7). It specifies the quantity of images used in an acquisition process.

Examples:

 

Label: has_number_of_picture
—--------------------------
Y16: has number of picture
Inverse: Y16-Inverse: is number of pictures of
Label: "is number of pictures of"
Domain: F41 Number of Picture
Range: F7 Picture Set

—------------------------------------------------------------------------


Y17: has acquisition operator
URI: https://photogrammetry.altervista.org/items/show/208 
Subproperty of: P14 carried out by

Domain: F2 Acquisition
Range: F37 Survey Operator

Scope Note:
This property links the acquisition process (F2) to the survey operator (F37) responsible for carrying out the data collection. It defines the role of the person or team who performed the acquisition.

Examples:

 
Label: has_acquisition_operator
—--------------------------
Y17: has acquisition operator
Inverse: Y17-Inverse: is operator of acquisition
Label: "is operator of acquisition"
Domain: F37 Survey Operator
Range: F2 Acquisition

—------------------------------------------------------------------------

Y18: has place of acquisition
URI: https://photogrammetry.altervista.org/items/show/209 
Subproperty of: P161 has spatial projection

Domain: F2 Acquisition
Range: F42 Place of Acquisition

Scope Note:
This property refers to the specific location (F42) where the acquisition event (F2) took place. It identifies the spatial setting or area in which the survey or documentation occurred.

Examples:

 
Label: has_place_of_acquisition
—--------------------------
Y18: has place of acquisition
Inverse: Y18-Inverse: is acquisition place of
Label: "is acquisition place of"
Domain: F42 Place of Acquisition
Range: F2 Acquisition

—------------------------------------------------------------------------


Y19: has date of acquisition
URI: https://photogrammetry.altervista.org/items/show/210 
Subproperty of: P4 has time span

Domain: F2 Acquisition
Range: F43 Survey Date

Scope Note:
This property identifies the date (F43) on which the acquisition process (F2) took place. It specifies when the data collection or survey was performed.

Examples:

 
Label:  has_date_of_acquisition
—----------------------------------------
Y19: has date of acquisition
Inverse: Y19-Inverse: is acquisition date of
Label: "is acquisition date of"
Domain: F43 Survey Date
Range: F2 Acquisition

—------------------------------------------------------------------------


Y20: has acquisition description
URI: https://photogrammetry.altervista.org/items/show/211 
Subproperty of: P3 has note

Domain: F2 Acquisition
Range: F44 Acquisition Description

Scope Note:
This property refers to a description (F44) of the acquisition event (F2). It provides additional notes or commentary on the method, conditions, or purpose of the data collection.

Examples:

 
Label: has_acquisition_description
—----------------------------------------

Y20: has acquisition description
Inverse: Y20-Inverse: is acquisition description of
Label: "is acquisition description of"
Domain: F44 Acquisition Description
Range: F2 Acquisition

—------------------------------------------------------------------------

Y21: has coordinates of acquisition
URI: https://photogrammetry.altervista.org/items/show/212 
Subproperty of: P169 defines spacetime volume

Domain: F45 Acquisition Coordinates
Range: F2 Acquisition

Scope Note:
This property specifies the geographic coordinates (F45) at which the acquisition event (F2) occurred. It links the acquisition process to the precise spatial coordinates where the data collection took place.

Examples:
 
Label: has_coordinates_of_acquisition
—------------------------------------
Y21: has coordinates of acquisition
Inverse Property: Y21-Inverse: "is acquisition coordinates for
Domain (Inverse): F2 Acquisition
Range (Inverse): F45 Acquisition Coordinates

Scope Note (Inverse):
This inverse property indicates that a set of Acquisition Coordinates (F45) serves as the spatial reference for a particular Acquisition (F2). It highlights the relationship from the perspective of coordinates, specifying for which acquisition event they apply.

Label (Inverse): is_acquisition_coordinates_for


—------------------------------------------------------------------------


Y22: had acquisition input
URI: https://photogrammetry.altervista.org/items/show/213 
Subproperty of: L10 had input
Domain: F3 Processing
Range: F25 Acquisition Raw Data

Scope Note:
This property links the processing phase (F3) to the acquisition raw data (F25) used as input for the processing.

Example:
A processing phase F3 Processing has as input F25 Acquisition Raw Data, which was generated by a laser scan.

Label: had_acquisition_input
—----------------------------------------
Y22: had acquisition input
Inverse Property: Y22-Inverse: is acquisition input of
Domain (Inverse): F25 Acquisition Raw Data
Range (Inverse): F3 Processing

Scope Note (Inverse):
This inverse property shows that a set of Acquisition Raw Data (F25) acts as the input for a specific Processing event (F3). It represents the relationship from the data’s standpoint, identifying which processing activity utilized it as input.

Label (Inverse): is_acquisition_input_of


—------------------------------------------------------------------------
Y23: has type of matching
URI: https://photogrammetry.altervista.org/items/show/214 
Subproperty of: P2 has type
Domain: F14 Matching Method
Range: F21 Matching Algorithm Type

Scope Note:
This property specifies the type of algorithm (F21) used during the matching method (F14) to align or correlate data.

Example:
The F14 Matching Method uses a F21 Matching Algorithm Type, such as a keypoint-based algorithm.
Label: has_type_of_matching
—-----------------------------------
Y23: has type of matching
Inverse Property: Y23-Inverse: is type of matching for
Domain (Inverse): F21 Matching Algorithm Type
Range (Inverse): F14 Matching Method

Scope Note (Inverse):
The inverse property states that a particular Matching Algorithm Type (F21) is applied by a certain Matching Method (F14). Thus, from the algorithm type’s perspective, it specifies which matching method employs it.

Label (Inverse): is_type_of_matching_for

—------------------------------------------------------------------------
Y24: happened on processing device
URI: https://photogrammetry.altervista.org/items/show/215 
Subproperty of: L12 happened on device
Domain: F3 Processing, F56  Mesh Reconstruction, F57  Texturing Mesh
Range: F10 Processing Device

Scope Note:
This property associates the processing phase (F3) with the processing device (F10) on which the processing occurred.

Example:
A processing phase F3 Processing happens on a F10 Processing Device, such as a high-performance server.

Label: happened_on_processing_device
—----------------------------------------
Y24: happened on processing device
Inverse Property: Y24-Inverse: is processing device for
Domain (Inverse): F10 Processing Device
Range (Inverse): F3 Processing, F56 Mesh Reconstruction, F57 Texturing Mesh

Scope Note (Inverse):
This inverse property indicates that a given Processing Device (F10) is the hardware on which various processing activities or subphases (F3, F56, F57) take place. It provides a device-centric view, showing which processes were executed on it.

Label (Inverse): is_processing_device_for

—------------------------------------------------------------------------
Y25: Processing is composed of
URI: https://photogrammetry.altervista.org/items/show/216 
Subproperty of: P9 consists of (forms part of)
Domain: F3 Processing
Range: F46 Matching / F47 Densification

Scope Note:
This property indicates that a processing phase (F3) is composed of subprocesses like matching (F46) or densification (F47).

Example:
A F3 Processing phase is composed of a F46 Matching phase followed by a F47 Densification phase, the property connect this relation.
Label: processing_is_composed_of
—----------------------------------------
Y25: Processing is composed of
Inverse Property: Y25-Inverse: is processing component of
Domain (Inverse): F46 Matching / F47 Densification
Range (Inverse): F3 Processing

Scope Note (Inverse):
From the perspective of a Matching (F46) or Densification (F47) activity, this inverse property indicates that such an activity forms part of a larger Processing (F3) procedure. It identifies these activities as components contributing to the overall processing phase.

Label (Inverse): is_processing_component_of


—------------------------------------------------------------------------
Y26: used processing software
URI: https://photogrammetry.altervista.org/items/show/217 
Subproperty of: L23 used software or firmware

Domain: F3 Processing, 56  Mesh Reconstruction, F57  Texturing Mesh
Range: F31 Processing Software

Scope Note:
This property identifies the software (F31) used during the processing phase (F3).

Example:
A F3 Processing phase uses F31 Processing Software, such as CloudCompare for handling point cloud data.
Label: used_processing_software
—------------------------------------------
Y26: used processing software
Inverse Property: Y26-Inverse: is processing software for
Domain (Inverse): F31 Processing Software
Range (Inverse): F3 Processing, F56 Mesh Reconstruction, F57 Texturing Mesh

Scope Note (Inverse):
This inverse property shows that a particular Processing Software (F31) is utilized by certain processing events or subphases, such as general processing (F3), mesh reconstruction (F56), or texturing (F57). It provides a software-centric perspective, revealing which processes depend on it.

Label (Inverse): is_processing_software_for

—------------------------------------------------------------------------
Y27: has method of densification
URI: https://photogrammetry.altervista.org/items/show/218 
Subproperty of: P33 used specific technique

Domain: F47 Densification
Range: F48 Densification Method

Scope Note:
This property links the densification process (F47) to the specific method (F48) used to increase the density of a point cloud or model.

Example:
A F47 Densification phase uses a F48 Densification Method, such as Multi-View Stereo (MVS) to increase point density.
Label: has_method_of_densification
—------------------------------------
Y27: has method of densification
Inverse Property: Y27-Inverse: is densification method for
Domain (Inverse): F48 Densification Method
Range (Inverse): F47 Densification

Scope Note (Inverse):
The inverse property states that a given Densification Method (F48) is applied within a Densification activity (F47). From the method’s viewpoint, it clarifies which densification activity employs it.

Label (Inverse): is_densification_method_for

—------------------------------------------------------------------------
Y28: has type of densification
URI: https://photogrammetry.altervista.org/items/show/219 
Subproperty of: P2 has type

Domain: F48 Densification Method
Range: F22 Densification Algorithm Type

Scope Note:
This property indicates the type of algorithm (F22) used in the densification method (F48) to enhance the density of a point cloud.

Example:
A F48 Densification Method uses a F22 Densification Algorithm Type, such as a dense feature matching algorithm.
Label: has_type_of_densification
—------------------------------------
Y28: has type of densification
Inverse Property: Y28-Inverse: is densification type for
Domain (Inverse): F22 Densification Algorithm Type
Range (Inverse): F48 Densification Method

Scope Note (Inverse):
This inverse property indicates that a certain Densification Algorithm Type (F22) is utilized by a specific Densification Method (F48). Thus, from the algorithm type’s perspective, it shows to which densification method it contributes.

Label (Inverse): is_densification_type_for

—------------------------------------------------------------------------
Y29: has matching input
URI: https://photogrammetry.altervista.org/items/show/220 
Subproperty of: L10 had input

Domain: F47 Densification
Range: F26 Point Cloud

Scope Note:
This property links the densification phase (F47) to the input point cloud (F26) used in the matching process.

Example:
A F47 Densification phase uses an input F26 Point Cloud, obtained from a preliminary laser scan.
Label: has_matching_input
—-------------------------------
Y29: has matching input
Inverse Property: Y29-Inverse: is matching input of
Domain (Inverse): F26 Point Cloud
Range (Inverse): F47 Densification

Scope Note (Inverse):
From the point cloud’s perspective, this inverse property reveals that the Point Cloud (F26) serves as input for a Densification (F47) activity. It clarifies which densification process relied on a specific point cloud dataset.

Label (Inverse): is_matching_input_of


—------------------------------------------------------------------------
Y30: has created point cloud
URI: https://photogrammetry.altervista.org/items/show/221 
Subproperty of: L11 has output

Domain: F46 Matching
Range: F26 Point Cloud

Scope Note:
This property links the matching phase (F46) to the creation of a point cloud (F26) as a result of the matching.

Example:
The relation that from F46 Matching process creates a F26 Point Cloud as its final output.
Label: has_created_point_cloud
—--------------------------------
Y30: has created point cloud
Inverse Property: Y30-Inverse: was created by matching
Domain (Inverse): F26 Point Cloud
Range (Inverse): F46 Matching

Scope Note (Inverse):
This inverse property states that a specific Point Cloud (F26) resulted from a Matching (F46) activity. Viewing from the point cloud’s perspective, it identifies which matching event generated it.

Label (Inverse): was_created_by_matching

—------------------------------------------------------------------------
Y31: has created densified point cloud
URI: https://photogrammetry.altervista.org/items/show/223 
Subproperty of: L11 has output

Domain: F47 Densification
Range: F27 Densified Point Cloud

Scope Note:
This property indicates that the result of the densification phase (F47) is a densified point cloud (F27).

Example:
The relation why a F47 Densification phase creates a F27 Densified Point Cloud with a higher density than the original input.
Label: has_created_densified_point_cloud
—--------------------------------------
Y31: has created densified point cloud
Inverse Property: Y31-Inverse: was created by densification
Domain (Inverse): F27 Densified Point Cloud
Range (Inverse): F47 Densification

Scope Note (Inverse):
From the densified point cloud’s perspective, this inverse property indicates which Densification (F47) process produced it. It helps trace the provenance and method behind the densified data set.

Label (Inverse): was_created_by_densification

—------------------------------------------------------------------------
Y32: has method of matching
URI: https://photogrammetry.altervista.org/items/show/222 
Subproperty of: P33 used specific technique

Domain: F46 Matching
Range: F14 Matching Method

Scope Note:
This property links the matching process (F46) to the specific matching method (F14) used.

Example:
The relation between a F46 Matching process and the F14 Matching Method, such as feature-based matching from images.
Label: has_method_of_matching
—-------------------------------------------
Y32: has method of matching
Inverse Property: Y32-Inverse: is matching method for
Domain (Inverse): F14 Matching Method
Range (Inverse): F46 Matching

Scope Note (Inverse):
This inverse property demonstrates that a particular Matching Method (F14) is employed by a Matching (F46) activity. From the method’s viewpoint, it identifies the matching event that utilizes it.

Label (Inverse): is_matching_method_for

—------------------------------------------------------------------------
Y33: has observed number of points
URI: https://photogrammetry.altervista.org/items/show/224 
This property is redundant and can be replaced by the superproperty 
- Y94: has observed number of points -

Subproperty of: P40 observed dimension
Domain: F50 Point Cloud Measurement
Range: F51 Point Cloud Number of Points

Scope Note:
This property associates a point cloud measurement (F50) with the observed number of points (F51).

Example:
A F50 Point Cloud Measurement records an observed number of F51 Point Cloud Number of Points, such as 1,000,000 points in a scan.
Label: pc_has_observed_number_of_points
—------------------------------------------------------------------------

Y34: was measured in number of points
URI: https://photogrammetry.altervista.org/items/show/225 
This property is redundant and can be replaced by the superproperty 
- Y95: was measured in number of points - 

Subproperty of: O24i was measured by
Domain: F26 Point Cloud
Range: F50 Point Cloud Measurement

Scope Note:
This property indicates that the number of points in a point cloud (F26) was measured in a point cloud measurement (F50).

Example:
A F26 Point Cloud was measured in an F50 Point Cloud Measurement, which recorded the total number of points.
Label: pc_was_measured_in_number_of_points 
—------------------------------------------------------------------------

Y35: has vertex quality assignment
URI: https://photogrammetry.altervista.org/items/show/226 
Subproperty of: P141i was assigned by

Domain: F26 Point Cloud
Range: F54 Point Cloud Quality Assignment

Scope Note:
This property links a point cloud (F26) to the assignment of its quality (F54), such as assessing the accuracy of each vertex.

Example:
A F26 Point Cloud has an assigned F54 Point Cloud Quality Assignment, indicating the quality of the vertices based on precision.
Label: has_vertex_quality_assignment
—------------------------------------------------------------------------

Y36: has Depth Noise Filtering
URI: https://photogrammetry.altervista.org/items/show/227 
Subproperty of: P141i was assigned by

Domain: F27 Dense Point Cloud
Range: F55 Depth Noise Filtering

Scope Note:
This property associates a dense point cloud (F27) with the application of a depth noise filtering technique (F55).

Example:
A F27 Dense Point Cloud undergoes F55 Depth Noise Filtering to remove noise from the depth data.
Label: has_depth_noise_filtering
—------------------------------------------------------------------------

Y37: has observed number of points (for dense point clouds)
URI: https://photogrammetry.altervista.org/items/show/228 
This property is redundant and can be replaced by the superproperty 
- Y94: has observed number of points -

Subproperty of: P40 observed dimension
Domain: F52 Dense Point Cloud Measurement
Range: F53 Dense Point Cloud Number of Points

Scope Note:
This property specifically refers to the number of points observed in a dense point cloud (F53) during a measurement (F52).

Example:
A F52 Dense Point Cloud Measurement records an observed number of F53 Dense Point Cloud Number of Points, such as 10,000,000 points in a densified scan.
Label: dpc_has_observed_number_of_points
—------------------------------------------------------------------------

Y38: was measured in number of points (for dense point clouds)
URI: https://photogrammetry.altervista.org/items/show/229 
This property is redundant and can be replaced by the superproperty 
- Y95: was measured in number of points - 

Subproperty of: O24i was measured by
Domain: F27 Dense Point Cloud
Range: F52 Dense Point Cloud Measurement

Scope Note:
This property relates a dense point cloud (F27) to the measurement of its number of points (F52).

Example:
A F27 Dense Point Cloud was measured in an F52 Dense Point Cloud Measurement, which recorded the number of points after densification.
Label: dpc_was_measured_in_number_of_points
—------------------------------------------------------------------------

Y39: has Sampling Points Range
URI: https://photogrammetry.altervista.org/items/show/230 
Subproperty of: P141i was assigned by
Domain: F27 Dense Point Cloud
Range: F49 Near Sample Point Range

Scope Note:
This property indicates the range of points in the dense point cloud (F27) near a sample point range (F49).

Example:
The relation that connect a F27 Dense Point Cloud that has a F49 Near Sample Point Range, describing the spread of sampling points in the dataset.
Label: has_sampling_points_range
—------------------------------------------------------------------------

Y40: has processing operator
URI: https://photogrammetry.altervista.org/items/show/231 
Subproperty of: P14 carried out by
Domain: F3 Processing
Range: F38 Processing Operator

Scope Note:
This property connects a processing phase (F3) to the operator (F38) who performed the processing.

Example:
A F3 Processing phase is carried out by a F38 Processing Operator, such as an engineer overseeing the data processing.
Label: has_processing_operator
—------------------------------------------------------------------------

Y41: used Phase Instruction
URI: https://photogrammetry.altervista.org/items/show/232 
Subproperty of: P33 used specific technique
Domain: F3 Processing
Range: F34 Processing Phase

Scope Note:
This property links the processing phase (F3) to the instructions (F34) used during that phase.

Example:
A F3 Processing phase uses specific F34 Processing Phase Instructions, detailing how to process a point cloud such as the BeAPG Protocol in the processing of AFMNM005 (Lauro 2019).
Label: used_processing_phase_instruction
—------------------------------------------------------------------------

Y42: was continued by Modelling phase
URI: https://photogrammetry.altervista.org/items/show/233 
This property is redundant and can be replaced by the superproperty 
-Y93 was continued by subsequent phase-
Subproperty of: P134i was continued by
Domain: F3 Processing
Range: F4 Modelling

Scope Note:
This property indicates that a processing phase (F3) was followed by a modelling phase (F4).

Example:
A F3 Processing phase was continued by an F4 Modelling phase, where a 3D model was generated from the processed data.
Label: was_continued_by_modelling_phase


—------------------------------------------------------------------------
Y43: has type of texturing
URI: https://photogrammetry.altervista.org/items/show/234 
Subproperty of: P2 has type
Domain: F16 Texturing Method
Range: F24 Texturing Type

Scope Note:
This property relates a texturing method (F16) to the type of texturing (F24) applied, such as UV mapping or procedural texturing.

Example:
A F16 Texturing Method has a F24 Texturing Type, such as UV Mapping applied to a 3D model.
Label: has_type_of_texturing
—------------------------------------------------------------------------

Y44: has type of reconstruction
URI: https://photogrammetry.altervista.org/items/show/235 
Subproperty of: P2 has type
Domain: F15 Reconstruction Method
Range: F23 Reconstruction Algorithm Type

Scope Note:
This property links a reconstruction method (F15) to the type of algorithm used for the reconstruction (F23), such as volumetric or point-based reconstruction.

Example:
A F15 Reconstruction Method uses a F23 Reconstruction Algorithm Type, such as a volumetric method for mesh creation.
Label: has_type_of_reconstruction
—------------------------------------------------------------------------

Y45: point cloud input
URI: https://photogrammetry.altervista.org/items/show/236 
Subproperty of: L10 had input
Domain: F56 Mesh Reconstruction
Range: F27 Densified Point Cloud

Scope Note:
This property connects a mesh reconstruction process (F56) with the input densified point cloud (F27) used to create the mesh.

Example:
A F56 Mesh Reconstruction process takes in a F27 Densified Point Cloud as input for generating a 3D mesh.
Label: point_cloud_input


—------------------------------------------------------------------------

Y46: has created 3D Mesh
URI: https://photogrammetry.altervista.org/items/show/237 
Subproperty of: L11 has output
Domain: F56 Mesh Reconstruction
Range: F28 3D Mesh

Scope Note:
This property indicates that the output of a mesh reconstruction process (F56) is a 3D mesh (F28).

Example:
A F56 Mesh Reconstruction process has created a F28 3D Mesh representing the geometry of the scanned object.
Label: has_created_tridimensional_mesh
—------------------------------------------------------------------------

Y47: has method of reconstruction
URI: https://photogrammetry.altervista.org/items/show/238 
Subproperty of: P33 used specific technique
Domain: F56 Mesh Reconstruction
Range: F15 Reconstruction Method

Scope Note:
This property associates a mesh reconstruction process (F56) with the specific reconstruction method (F15) it used, such as surface reconstruction or volumetric reconstruction.

Example:
A F56 Mesh Reconstruction process uses a F15 Reconstruction Method, such as a surface reconstruction technique.
Label: has_method_of_reconstruction
—------------------------------------------------------------------------

Y48: has method of texturing
URI: https://photogrammetry.altervista.org/items/show/239 
Subproperty of: P33 used specific technique
Domain: F57 Texturing Mesh
Range: F16 Texturing Method

Scope Note:
This property connects a texturing process (F57) with the specific texturing method (F16) it employs, such as UV mapping or projective texturing.

Example:
A F57 Texturing Mesh process uses a F16 Texturing Method, such as UV Mapping for applying textures to a 3D mesh.
Label: has_method_of_texturing
—------------------------------------------------------------------------

Y49: has created Digital Twin
URI: https://photogrammetry.altervista.org/items/show/240 
Subproperty of: L11 has output
Domain: F58 Modifying Mesh
Range: F100 Digital Twin

Scope Note:
This property indicates that the output of a mesh modification process (F58) is a digital twin (F100), which is a precise digital replica of a real-world object.

Example:
A F58 Modifying Mesh process has created a F100 Digital Twin, accurately representing the physical object.
Label: has_created_digital_twin
—------------------------------------------------------------------------

Y50: happened on modelling device
URI: https://photogrammetry.altervista.org/items/show/241 
Subproperty of: L12 happened on device
Domain: F58 Modifying Mesh
Range: F11 Modelling Device

Scope Note:
This property connects a mesh modification process (F58) with the device (F11) on which it was carried out, such as a computer or a specific 3D modelling workstation.

Example:
A F58 Modifying Mesh process happened on an F11 Modelling Device, such as a high-end 3D modelling workstation.
Label: happened_on_modelling_device


—------------------------------------------------------------------------

Y51: Modelling is composed of
URI: https://photogrammetry.altervista.org/items/show/242 
Subproperty of: P9 consists of
Domain: F4 Modelling
Range: F56 Mesh Reconstruction / F57 Texturing Mesh / F58 Modifying Mesh

Scope Note:
This property indicates that a modelling process (F4) is composed of various sub-processes such as mesh reconstruction (F56), texturing (F57), and modifying mesh (F58).

Example:
A F4 Modelling process consists of F56 Mesh Reconstruction, F57 Texturing Mesh, and F58 Modifying Mesh, to complete the full 3D model.
Label: modelling_is_composed_of
—------------------------------------------------------------------------

Y52: 3D mesh input
URI: https://photogrammetry.altervista.org/items/show/243 
Subproperty of: L10 had input
Domain: F28 3D Mesh
Range: F57 Texturing Mesh

Scope Note:
This property links a 3D mesh (F28) as input for a texturing mesh process (F57).

Example:
A F28 3D Mesh is the input for a F57 Texturing Mesh process, where textures will be applied to the mesh.
Label: tridimensional_mesh_input
—------------------------------------------------------------------------

Y53: Textured 3D mesh input
URI: https://photogrammetry.altervista.org/items/show/244 
Subproperty of: L10 had input
Domain: F29 Textured Mesh
Range: F58 Modifying Mesh

Scope Note:
This property connects a textured 3D mesh (F29) as input for a mesh modification process (F58).

Example:
A F29 Textured Mesh serves as the input for an F58 Modifying Mesh process, where the textured mesh will undergo further refinement.
Label: textured_tridimensional_mesh_input
—------------------------------------------------------------------------

Y54: has created textured 3D mesh
URI: https://photogrammetry.altervista.org/items/show/245 
Subproperty of: L11 has output
Domain: F57 Texturing Mesh
Range: F29 Textured Mesh

Scope Note:
This property indicates that the output of a texturing mesh process (F57) is a textured 3D mesh (F29).

Example:
A F57 Texturing Mesh process has created a F29 Textured Mesh, which includes both geometry and applied textures.

Label: has_created_textured_tridimensional_mesh

—------------------------------------------------------------------------
Y55: has digital scale
URI: https://photogrammetry.altervista.org/items/show/246 
Subproperty of: P43 has dimension
Domain: F100 Digital Twin
Range: F59 Digital Scale

Scope Note:
This property links a digital twin (F100) to its digital scale (F59), which represents the measurement scale in the digital environment.

Example:
A F100 Digital Twin has a F59 Digital Scale of 1:50, representing the scale used to model the digital twin.
Label: has_digital_scale
—------------------------------------------------------------------------

Y56: has smoothing filter
URI: https://photogrammetry.altervista.org/items/show/247 
Subproperty of: P141i was assigned by
Domain: F28 3D Mesh
Range: F60 Smoothing Filter

Scope Note:
This property connects a 3D mesh (F28) with the smoothing filter (F60) applied to reduce noise or irregularities in the mesh.

Example:
A F28 3D Mesh has been assigned a F60 Smoothing Filter to soften rough areas in the model.
Label:  has_smoothing_filter
—------------------------------------------------------------------------

Y57: has color balance/multiband
URI: https://photogrammetry.altervista.org/items/show/248 
Subproperty of: P141i was assigned by
Domain: F62 Texture Set of 3D Mesh
Range: F61 Color Balance/Multiband Texture

Scope Note:
This property relates a set of textures on a 3D mesh (F62) to the color balance or multiband processing (F61) used in its creation.

Example:
A F62 Texture Set of 3D Mesh has a F61 Color Balance/Multiband Texture applied to achieve a natural and balanced appearance.
Label: has_color_balance_or_multiband
—------------------------------------------------------------------------

Y58: has number of texture
URI: https://photogrammetry.altervista.org/items/show/249 
(Not a subproperty)
Domain: F62 Texture Set of 3D Mesh
Range: F63 Number of Texture

Scope Note:
This property defines the number of textures (F63) present in a texture set (F62) for a 3D mesh.

Example:
A F62 Texture Set of 3D Mesh has F63 Number of Texture, indicating the number of individual texture files used in the set.
Label: has_number_of_texture
—------------------------------------------------------------------------

Y59: is texture set of 
URI: https://photogrammetry.altervista.org/items/show/250 
Subproperty of: P106i forms part of
Domain: F62 Texture Set of 3D Mesh
Range: F29 Textured Mesh

Scope Note:
This property indicates that a texture set (F62) forms part of a textured 3D mesh (F29), contributing to its visual representation.

Example:
A F62 Texture Set of 3D Mesh is part of a F29 Textured Mesh, providing the texture details for the mesh.
Label: is_texture_set_of


—------------------------------------------------------------------------

Y60: has modelling description
URI: https://photogrammetry.altervista.org/items/show/251 
Subproperty of: P3 has note
Domain: F4 Modelling
Range: F64 Modelling Description

Scope Note:
This property links a modelling process (F4) with a descriptive note (F64) detailing the process, method, or specifics about the model.

Example:
A F4 Modelling process has a F64 Modelling Description, such as an explanation of the procedural steps used to create the 3D model.
Label:  has_modelling_description


—------------------------------------------------------------------------

Y61: used modelling software
URI: https://photogrammetry.altervista.org/items/show/252 
Subproperty of: L23 used software or firmware
Domain: F58 Modifying 3D Mesh
Range: F32 Modelling Software

Scope Note:
This property connects a 3D mesh modification process (F58) with the software (F32) used during the modification.

Example:
A F58 Modifying 3D Mesh process used F32 Modelling Software, such as Blender or Autodesk Maya, to alter the 3D model.
Label: used_modifying_software
—------------------------------------------------------------------------

Y62: has modelling operator
URI: https://photogrammetry.altervista.org/admin/items/show/253 
Subproperty of: P14 carried out by
Domain: F4 Modelling
Range: F39 Modelling Operator

Scope Note:
This property relates a modelling process (F4) to the operator (F39) responsible for carrying out the modelling work.

Example:
A F4 Modelling process was carried out by a F39 Modelling Operator, such as a skilled 3D artist or modeller.
Label: has_modifying_operator
—------------------------------------------------------------------------

Y63: has date of modelling
URI: https://photogrammetry.altervista.org/items/show/254 
Subproperty of: P4 has time span
Domain: F58 Modifying Mesh
Range: F65 Modelling Date

Scope Note:
This property connects a 3D mesh modification process (F58) with the date (F65) on which the modification was carried out.

Example:
A F58 Modifying Mesh process has a F65 Modelling Date, such as "August 12, 2023," marking when the model was altered.
Label: has_date_of_acquisition
—------------------------------------------------------------------------

Y65: Modelling is influenced by
URI: https://photogrammetry.altervista.org/items/show/255 
Subproperty of: P15i influenced
Domain: F58 Modifying Mesh
Range: F66 Modelling Determination / F67 Modelling Elimination

Scope Note:
This property links a 3D mesh modification process (F58) to the factors (F66/F67) that influenced or eliminated aspects of the model.

Example:
A F58 Modifying Mesh process is influenced by a F66 Modelling Determination, such as a specific requirement to improve edge flow or reduce polygon count in the model.

Label: modifying_is_influenced_by
—------------------------------------------------------------------------

Y66: is Digital Twin physical carrier
URI: https://photogrammetry.altervista.org/admin/items/show/256 
Subproperty of: L19 stores
Domain: F68 Model Physical Carrier
Range: F100 Digital Twin

Scope Note:
This property links the physical carrier of a model (F68), such as a hard drive or other storage medium, to the digital twin (F100) it contains.

Example:
A F68 Model Physical Carrier (a hard drive) stores a F100 Digital Twin of a heritage monument.
Label: is_tridimensional_digital_twin_physical_carrier
—------------------------------------------------------------------------


Y67: was continued by Exporting phase
URI: https://photogrammetry.altervista.org/items/show/257 
This property is redundant and can be replaced by the superproperty 
-Y93 was continued by subsequent phase-
Subproperty of: P134i was continued by
Domain: F4 Modelling
Range: F5 Exporting

Scope Note:
This property indicates that a modelling process (F4) was continued by an exporting phase (F5), marking the transition from modelling to exporting the model into a usable format.

Example:
A F4 Modelling process was continued by a F5 Exporting phase, where the model was exported in a standard format, like OBJ or STL.
Label:  was_continued_by_exporting_phase
—------------------------------------------------------------------------

Y68: has Textured 3D Model as input
URI: https://photogrammetry.altervista.org/items/show/258 
Subproperty of: L10 had input
Domain: F5 Exporting
Range: F29 Textured 3D Model, F100 Digital Twin

Scope Note:
This property relates the exporting phase (F5) to a textured 3D model (F29) that serves as input during the exporting process.

Example:
During the F5 Exporting process, a F29 Textured 3D Model was used as input for generating a final 3D product.
Label: has_textured_tridimensional_model_as_input
—------------------------------------------------------------------------


Y69: has Digital Twin as output
URI: https://photogrammetry.altervista.org/items/show/259 
Subproperty of: L11 had output
Domain: F5 Exporting
Range: F100 Digital Twin

Scope Note:
This property indicates that the result of the exporting phase (F5) is a digital twin (F100), which is the digital output of the process.

Example:
A F5 Exporting phase has produced a F100 Digital Twin, representing the final exported digital copy of the model.
Label: has_tridimensional_digital_twin_as_output


—------------------------------------------------------------------------


Y70: Final Use of 3D Model consists of
URI: https://photogrammetry.altervista.org/items/show/260 
Subproperty of: P9 consists of
Domain: F5 Exporting
Range: F71 Final Use of 3D Model

Scope Note:
This property indicates that the final use of the 3D model (F71) is defined or composed during the exporting phase (F5).

Example:
The F5 Exporting phase defines that the F71 Final Use of the 3D Model will be for 3D printing.
Label: exporting_tridimensional_digital_twin_consists_of 
—------------------------------------------------------------------------


Y71: has number of final destination
URI: https://photogrammetry.altervista.org/items/show/261 
(Not a subproperty)
Domain: F71 Final Use of 3D Model
Range: F70 Number of Final Destination

Scope Note:
This property indicates the number of final destinations (F70) for the 3D model based on the final use (F71).

Example:
The F71 Final Use of the 3D Model has F70 Number of Final Destination, such as three different output formats: video rendering, printing, and research.
Label: tridimensional_digital_twin_has_number_of_use
—------------------------------------------------------------------------


Y72: had final use output
URI: https://photogrammetry.altervista.org/items/show/262 
Subproperty of: L11 had output
Domain: F71 Final Use of 3D Model
Range: F72 3D Model Video Rendering, F76 3D Model for 3D Print, F81 3D Model for G.I.S., F84 3D Model for Prospectuses, F88 3D Model for Research, F91 3D Model for Interactive, F94 3D Model for Database

Scope Note:
This property connects the final use of a 3D model (F71) to its specific output form (F72, F76, F81, etc.), depending on the intended application of the model.

Example:
The F71 Final Use of the 3D Model has produced F72 3D Model Video Rendering and F76 3D Model for 3D Print as output formats for different applications.
Label: exporting_has_output

—------------------------------------------------------------------------

Y73: had rendering as input
URI: https://photogrammetry.altervista.org/items/show/263 
Subproperty of: L10 had input
Domain: F73 Editing Video
Range: F72 3D Model Video Rendering

Scope Note:
This property links the rendering process (as part of video creation) to the video editing software that serves as the input for further editing.

Example:
The Editing Video process had a Rendering as input, handled by Video Editing Software such as Adobe Premiere.
Label: had_rendering_as_input
—------------------------------------------------------------------------

Y74: use video editing software
URI: https://photogrammetry.altervista.org/items/show/275 
Subproperty of: L23 used software or firmware
Domain: F73 Editing Video
Range: F74 Video Editing Software

Scope Note:
This property specifies that the video editing process (Editing Video) used specific video editing software.

Example:
The Editing Video phase used Video Editing Software like Final Cut Pro to edit a 3D rendering video.
Label: used_video_editing_software
—------------------------------------------------------------------------

Y75: had Video output
URI: https://photogrammetry.altervista.org/items/show/276 
Subproperty of: L11 had output
Domain: F73 Editing Video
Range: F75 Project Video

Scope Note:
This property indicates that the video editing process (Editing Video) results in a project video (Project Video) as its output.

Example:
The Editing Video process produced a Project Video as output, which can be used for presentation or further rendering. 
Label:  had_video_output
—------------------------------------------------------------------------

Y76: printing based on
URI: https://photogrammetry.altervista.org/items/show/277 
Subproperty of: P17 was motivated by
Domain: F77 Printing Digital Twin
Range: F76 3D Model for 3D Print

Scope Note:
This property shows that the printing process of a digital twin (Printing Digital Twin) is motivated by or based on a specific 3D model intended for 3D printing.

Example:
The Printing Digital Twin process is based on the 3D Model for 3D Print that was developed during the modelling phase.
Label: printing_based_on
—------------------------------------------------------------------------

Y77: has printed physical digital twin
URI: https://photogrammetry.altervista.org/items/show/278 
Subproperty of: P108 has produced
Domain: F77 Printing Digital Twin
Range: F80 Printed Digital Twin

Scope Note:
This property links the printing process of a digital twin (Printing Digital Twin) to the final physical output, a Printed Digital Twin.

Example:
The Printing Digital Twin process produced a Printed Digital Twin, representing the physical counterpart of the digital model.
Label: has_printed_physical_digital_twin
—------------------------------------------------------------------------

Y78: used specific printing machine
URI: https://photogrammetry.altervista.org/items/show/279 
Subproperty of: P16 used specific object
Domain: F77 Printing Digital Twin
Range: F79 Printing Device

Scope Note:
This property defines the specific printing machine (Printing Device) used in the process of printing a digital twin (Printing Digital Twin).

Example:
The Printing Digital Twin process used a Printing Device like an SLS 3D printer.
Label: used_specific_printing_machine
—------------------------------------------------------------------------

Y79: consists of printing material
URI: https://photogrammetry.altervista.org/items/show/280 
Subproperty of: P45 consists of
Domain: F80 Printed Digital Twin
Range: F78 Material for 3D Printed

Scope Note:
This property indicates the materials (Material for 3D Printed) used in the creation of a Printed Digital Twin.

Example:
The Printed Digital Twin consists of Material for 3D Raw, such as PLA or resin.
Label: consists_of_printing_material
—------------------------------------------------------------------------

Y80: is in GIS  (GIS hosts the model)
URI: https://photogrammetry.altervista.org/items/show/281 
Subproperty of: P106i forms part of
Domain: F81 3D Model for GIS
Range: F82 Reference GIS System

Scope Note:
This property indicates that a 3D model for GIS (3D Model for GIS) is integrated within a specific GIS system (Reference GIS System).

Example:
The 3D Model for GIS is included in a Reference GIS System like ArcGIS for geospatial analysis.
Label: is_in_GIS
—------------------------------------------------------------------------

Y81: used GIS software
URI: https://photogrammetry.altervista.org/items/show/282 
Subproperty of: L23 used software or firmware
Domain: F82 Reference GIS System
Range: F83 GIS Software

Scope Note:
This property specifies the GIS software (GIS Software) that was used to manage or process the 3D model within the GIS system.

Example:
The Reference GIS System used GIS Software such as QGIS to integrate the 3D model with geographic data.
Label: used_GIS_software
—------------------------------------------------------------------------

Y82: had model prospectuses for CAD as input
URI: https://photogrammetry.altervista.org/items/show/283 
Subproperty of: L10 had input
Domain: F85 CAD Analysis
Range: F87 3D Model for Prospectuses

Scope Note:
This property indicates that the CAD analysis phase (CAD Analysis) used a 3D model designed for prospectuses (3D Model for Prospectuses) as an input.

Example:
 
Label: had_model_prospectus_as_input
—------------------------------------------------------------------------

Y83: used CAD software
URI: https://photogrammetry.altervista.org/items/show/284 
Subproperty of: L23 used software
Domain: F85 CAD Analysis
Range: F86 Software CAD

Scope Note:
This property specifies that the CAD analysis phase (CAD Analysis) used a specific CAD software (Software CAD) for its operations.

Example:
 
Label: used_CAD_software
—------------------------------------------------------------------------

Y84: had prospectus output
URI: https://photogrammetry.altervista.org/items/show/285 
Subproperty of: L11 had output
Domain: F85 CAD Analysis
Range: F87 3D Model Prospectus

Scope Note:
This property indicates that the CAD analysis (CAD Analysis) produced a 3D model prospectus (3D Model Prospectus) as its output.

Example:
  
Label: had_prospectus_output
—------------------------------------------------------------------------

Y85: had archaeometric input
URI: https://photogrammetry.altervista.org/items/show/274 
Subproperty of: L10 had input
Domain: F89 Project Analysis
Range: F88 Archaeometric 3D Model

Scope Note:
This property specifies that the project analysis (Project Analysis) used an archaeometric 3D model (Archaeometric 3D Model) as an input for detailed material or structural analysis.

Example:
  
Label: had_archaeometric_input
—------------------------------------------------------------------------

Y86: had data log analysis output
URI: https://photogrammetry.altervista.org/items/show/273 
Subproperty of: L11 had output
Domain: F89 Project Analysis
Range: F90 Data Log Analysis

Scope Note:
This property indicates that the project analysis phase (Project Analysis) resulted in a data log analysis (Data Log Analysis) as its output.

Example:
  
Label: had_data_log_analysis_output
—------------------------------------------------------------------------

Y87: had 3D model interactive as input
URI: https://photogrammetry.altervista.org/items/show/272 
Subproperty of: L10 had input
Domain: F92 Interactive Project Implementation
Range: F91 3D Model for Interactive

Scope Note:
This property shows that the interactive project (Interactive Project) used a 3D model designed for interactive use (3D Model for Interactive) as its input.

Example:
  
Label: had_interactive_tridimensional_model_as_input
—------------------------------------------------------------------------

Y88: used interactive software
URI: https://photogrammetry.altervista.org/items/show/271 
Subproperty of: L23 used software
Domain: F92 Interactive Project Implementation
Range: F93 Interactive Software

Scope Note:
This property indicates that the interactive project (Interactive Project) used interactive software (Interactive Software) to facilitate the project's immersive features.

Example:

Label: used_interactive_software
—------------------------------------------------------------------------

Y89: had 3D model for database as input
URI: https://photogrammetry.altervista.org/items/show/270 
Subproperty of: L10 had input
Domain: Database Project
Range: 3D Model for Database

Scope Note:
This property shows that the database project (Database Project) used a 3D model meant for database storage (3D Model for Database) as its input.

Example:
 
Label: had_model_for_database_as_input
—------------------------------------------------------------------------

Y90: used database software/architecture
URI: https://photogrammetry.altervista.org/items/show/269 
Subproperty of: L23 used software
Domain: Database Project
Range: Database Architecture

Scope Note:
This property indicates that the database project (Database Project) used specific database software or architecture (Database Architecture) for managing and storing data.

Example:
  
Label: used_database_architecture
—------------------------------------------------------------------------

Y91: had 3D model for AR as input
URI: https://photogrammetry.altervista.org/items/show/268 
Subproperty of: L10 had input
Domain: AR/MR Project
Range: 3D Model for Augmented Reality

Scope Note:
This property specifies that the AR/MR project (AR/MR Project) used a 3D model for augmented reality (3D Model for Augmented Reality) as its input.

Example:
 
Label: had_tridimensional_model_for_augmented_reality_as_input
—------------------------------------------------------------------------

Y92: used AR/MR software
URI: https://photogrammetry.altervista.org/items/show/267 
Subproperty of: L23 used software
Domain: AR/MR Project
Range: AR Software Modelling

Scope Note:
This property indicates that the AR/MR project (AR/MR Project) used augmented reality software (AR Software Modelling) for developing and presenting AR content.

Example:


Label: used_augmented_or_mixed_reality_software
—------------------------------------------------------------------------
Y93: was continued by subsequent phase
URI: https://photogrammetry.altervista.org/items/show/266 
Subproperty of: 
P134i was continued by
Domain: F101 Survey Phase
Range: F101 Survey Phase

Scope Note:
This property connects one Survey Phase (F101) to a subsequent Survey Phase (F101), marking the progression of the survey process from one phase to another. The aim of this property is to articulate the sequence of phases involved in a survey, often defined by different design choices or procedural steps. It highlights how a given survey phase transitions into a new one, either in terms of methodology or operational focus.

Examples:
A Survey Phase focused on preliminary data gathering was continued by a subsequent Survey Phase dedicated to higher-resolution data acquisition.

Label: was_continued_by_subsequent_phase
—------------------------------------------------------------------------
Y94: has observed number of points
URI: https://photogrammetry.altervista.org/items/show/265 
Subproperty of: P40 observed dimension
Domain: F50 Point Cloud Measurement, F52 Dense Point Cloud Measurement
Range: F51 Point Cloud Number of Points, F53 Dense Point Cloud Number of Points

Scope Note:
This property refers to the number of points observed in a Point Cloud (F51) or Dense Point Cloud (F53) during a Point Cloud Measurement (F50) or a Dense Point Cloud Measurement (F52). It captures the quantity of individual data points that have been identified and recorded in the measurement phase, allowing for the specification of the point cloud's resolution.

Examples:

A F50 Point Cloud Measurement records an observed number of F51 Point Cloud Number of Points, such as 500,000 points in a basic scan.
A F52 Dense Point Cloud Measurement records an observed number of F53 Dense Point Cloud Number of Points, such as 12,000,000 points in a densified scan.
Label:  has_observed_number_of_points

—------------------------------------------------------------------------
Y95: was measured in number of points
URI: https://photogrammetry.altervista.org/items/show/264 
Subproperty of: O24 measured 
Domain: F26 Point Cloud, F27 Dense Point Cloud
Range: F50 Point Cloud Measurement, F52 Dense Point Cloud Measurement

Scope Note:
This property connects a Point Cloud (F26) or a Dense Point Cloud (F27) with the corresponding Point Cloud Measurement (F50) or Dense Point Cloud Measurement (F52), indicating that the cloud was measured in terms of the number of points it contains. It defines the relationship between the point cloud as a data set and the measurement process that captures its resolution by counting the number of individual points within the cloud.

Examples:

A F26 Point Cloud was measured in F50 Point Cloud Measurement, which recorded 600,000 points in a typical scan.
A F27 Dense Point Cloud was measured in F52 Dense Point Cloud Measurement, which recorded 15,000,000 points in a high-resolution scan.
Label: was_measured_in_number_of_points

—------------------------------------------------------------------------



Object Property & Data Property 

Object Properties :
Y1: is acquired object of
Y2: had pictures input
Y3: has Type Of Acquisition
Y4: has dominant geometry type
Y5: has scale type
Y6: used trajectory
Y7: has method of acquisition
Y8: happened on acquisition device
Y9: has acquisition device type
Y10: has created raw data
Y11: used acquisition software
Y12: was continued by Processing Phase
Y13: used Acquisition Instruction
Y14: stores acquisition Picture
Y15: is composed of picture
Y17: has acquisition operator
Y18: has place of acquisition
Y22: had acquisition input
Y23: has type of matching
Y24: happened on processing device
Y25: Processing is composed of
Y26: used processing software
Y27: has method of densification
Y28: has type of densification
Y29: has matching input
Y30: has created point cloud
Y31: has created densified point cloud
Y32: has method of matching
Y35: has vertex quality assignment
Y36: has Depth Noise Filtering
Y40: has processing operator
Y41: used Phase Instruction
Y42: was continued by Modelling phase
Y43: has type of texturing
Y44: has type of reconstruction
Y45: point cloud input
Y46: has created 3D Mesh
Y47: has method of reconstruction
Y48: has method of texturing
Y49: has created Digital Twin
Y50: happened on modelling device
Y51: Modelling is composed of
Y52: 3D mesh input
Y53: Textured 3D mesh input
Y54: has created textured 3D mesh
Y59: is texture set of
Y62: has modelling operator
Y65: Modelling is influenced by
Y66: is Digital Twin physical carrier
Y67: was continued by Exporting phase
Y68: has Textured 3D Model as input
Y69: has Digital Twin as output
Y70: Final Use of 3D Model consists of
Y72: had final use output
Y73: had rendering as input
Y74: use video editing software
Y75: had Video output
Y76: printing based on
Y77: has printed physical digital twin
Y78: used specific printing machine
Y80: is in GIS
Y81: used GIS software
Y82: had model prospectuses for CAD as input
Y83: used CAD software
Y84: had prospectus output
Y85: had archaeometric input
Y86: had data log analysis output
Y87: had 3D model interactive as input
Y88: used interactive software
Y89: had 3D model for database as input
Y90: used database software/architecture
Y91: had 3D model for AR as input
Y92: used AR/MR software
Y93: was continued by subsequent phase
Y39: has Sampling Points Range
Y55: has digital scale
Y56: has smoothing filter
Y57: has color balance/multiband
Data Properties:
Y16: has number of picture
Y19: has date of acquisition
Y20: has acquisition description
Y21: has coordinates of acquisition
Y33: has observed number of points
Y34: was measured in number of points
Y37: has observed number of points (for dense point clouds)
Y38: was measured in number of points (for dense point clouds)
Y58: has number of texture
Y60: has modelling description
Y63 has date of modelling
Y71: has number of final destination
Y94: has observed number of points
Y95: was measured in number of points


 
























 









References 
G. Artopoulos, et alii, Spatially-Organized Virtual Narratives of Contested Urban Space: Digital Methods of Mapping the Spatial Experience of Shared Heritage, Body Space Technology Journal

D. Abate, et alii., Virtual and physical re-composition of fragmented ecclesiastical frescoes using a photogrammetric approach. Proceedings of the International Society for Photogrammetry and Remote Sensing, Comission VI, Prague, 2016

A. Uˇcakar et alii, 3D Digital Preservation, Presentation, and Interpretation of Wooden Cultural Heritage on the Example of Sculptures of the FormaViva Kostanjevica Na Krki Collection in Applied Science 12, 8445. https://doi.org/10.3390/app12178445 2022

Przemyslaw Klapa et al 2017 IOP Conf. Ser.: Earth Environ. Sci. 95 032007

Lauro, V.; Giovannangelo, M.; De Riggi, M.; Lanzaro, N.; Murtas, V. R.A.O. Project Recovery: Methods and Approaches for the Recovery of a Photographic Archive for the Creation of a Photogrammetric Survey of a Site Unreachable over Time. Heritage 2023, 6, 4710-4721. https://doi.org/10.3390/heritage6060250

A. Gruen , Remondino F., L Zhang., Photogrammetric reconstruction of the great Buddha of Bamiyan, Afghanistan, in  The Photogrammetric Record 2004

Vittorio Murtas, Vittorio Lauro, and Vincenzo Lombardo. 2023. Virtual Archaeology in a Multi-platform and Multi-lingual Setting. In Adjunct Proceedings of the 31st ACM Conference on User Modeling, Adaptation and Personalization (UMAP '23 Adjunct). Association for Computing Machinery, New York, NY, USA, 422–426. https://doi.org/10.1145/3563359.3596664

Polat N, Ulukavak M, Memduhoğlu A, Şenol H İ & Kaya Y (2020). UAV Based 3D Modeling
of Ancient Quarry Nearby the Göbeklitepe. Intercontinental Geoinformation Days (IGD),
252-255, Mersin, Turkey

E. Iadanza et alii, Semantic web technologies meet bim for accessing and understanding cultural heritage in The International Archives of the Photogrammetry, Remote Sensing and Spatial Information Sciences, Volume XLII-2/W9, 2019 8th Intl. Workshop 3D-ARCH “3D Virtual Reconstruction and Visualization of Complex Architectures”, 6–8 February 2019, Bergamo

 M. Douglass et alii, The Application of 3D Photogrammetry for In-Field Documentation of Archaeological Features, Cambridge University Press, 2017





Ontology and Thesaury References 

CIDOC-CRM
https://www.cidoc-crm.org/html/cidoc_crm_v7.1.3.html

CIDOC-CRMdig
https://www.cidoc-crm.org/extensions/crmdig/html/CRMdig_v4.0.html

CIDOC-CRMsci 
https://www.cidoc-crm.org/extensions/crmsci/html/CRMsci_v2.0.html

FOPPA 
https://protocol-foppa.jimdosite.com/
https://github.com/Vlauro/FOPPA

COSCHKR 
https://www.cosch.info/
https://gitlab.rlp.net/i3mainz/forschung/cosch-kr/cosch-kr-ontology



Manual of Acquisition 

FARO 
https://farotechnologies.mcoutput.com/focus-scanner/it-it/Default.htm




PODS 1_1_79


F106 Acquisition Location Type
URI: https://photogrammetry.altervista.org/items/show/286 
Subclass of: E55 Type

Scope Note:
The Acquisition Location Type class categorizes the setting in which data acquisition took place. It specifies whether the location was outdoors, indoors with natural lighting, indoors with controlled lighting, in a dark space (such as a cave), outdoors with no natural lighting, outdoors with supplementary artificial lighting, or entirely illuminated by artificial sources.

Examples:

An indoor environment with low light, such as a museum display room.
An outdoor archaeological site without additional lighting.

Label: acquisition_location_type

—--------------------------------------------------------------------------------------
F108 Calibration of the Instrument
URI: https://photogrammetry.altervista.org/items/show/287 
Subclass of: F2 Acquisition

Scope Note:
The Calibration of the Instrument class records the calibration process of the acquisition device, such as a camera, laser scanner, fixed-camera photogrammetry system (e.g., ATOS III), or LiDAR. This includes any calibration procedures conducted before acquisition or throughout the data capture process to ensure accuracy and reliability in measurement.

Examples:

Pre-acquisition calibration of a laser scanner.
Calibration of a fixed photogrammetry camera system for high-resolution artifact capture.

Label: Acquisition_InstrumentCalibration
—--------------------------------------------------------------------------

F109 Marker and Calibration Tools
URI: https://photogrammetry.altervista.org/items/show/288 
Subclass of: F9 Acquisition Device

Scope Note:
The Marker and Calibration Tools class encompasses all tools used for instrument calibration, including markers placed prior to acquisition (e.g., those required by fixed-camera systems like ATOS III) and those used during data capture (such as markers for software like Agisoft). This class also includes total station prisms and any external coordinate assignment tools.

Examples:

Markers used in photogrammetry software for real-time calibration.
Prisms applied in total station systems for external coordinate accuracy.

Label: AcquisitionDeviceMarker&Calibration

—----------------------------------------------------------------------------------------



PODS 1_2_2

F110 Processing Description
URI: https://photogrammetry.altervista.org/items/show/289 
Subclass of: E62_String

Scope Note:
The detailed description of the processes relating to the processing of the acquired raw data. The description includes the structural details of the processing device or point cloud extraction and their densification that have not found space in the other classes or that are specific to a particular acquisition or processing tool. To the extent that the acquisition and processing processes are integrated, the description must be replicated between the Processing Description class and the Acquisition Description.

Examples:

In the context of processing an archaeological find with the ATOS III scanner the following values ​​max_intersection_deviation (0.02 - 0.08), average_point_distance in Mesh (0.11321688668448972) were recorded using a Sensor ATOS III Rev.02 for an EllipseQuality generation of 0.25

Label: ProcessingDescription

—----------------------------------------------------------------------------------------

F111 Video Format Type
URI: https://photogrammetry.altervista.org/items/show/290 
Subclass of: E55_Type

Scope Note:
This class defines the type of video format used in a digital media object. Video format types can vary based on encoding standards and container formats, which can affect compatibility, quality, and file size. The choice of format is essential for ensuring the usability and performance of the video in different contexts, including playback on specific devices, streaming, and archival. Expressed, where possible, as a text string with one of the following options

AVI
MP4
MKV
MOV
FLV
WMV
WebM
MPG / MPEG
3GP
OGV
M4V
MXF
ASF
VOB
TS
F4V
RM / RMVB
AVCHD
HLS
DV
DivX


Examples:

MP4
AVI
MOV
MKV

Label: VideoRenderingFormatType


—----------------------------------------------------------------------------------------

F112 Video Resolution
URI: https://photogrammetry.altervista.org/items/show/291 
Subclass of: E54_Dimension

Scope Note:
This class represents the resolution of a video, which is defined as the number of pixels displayed in each dimension (width x height). Video resolution is a crucial factor affecting the quality and clarity of a video, as well as its file size. Higher resolutions provide better visual detail but require more storage and processing power. Common resolutions are often standardized and impact the video’s suitability for specific display types and use cases. Expressed, where possible, with an integer numeral value X an integer numeral value.

Examples:

1920x1080 (Full HD)
3840x2160 (4K UHD)
1280x720 (HD)

Label: VideoRenderingResolution


—----------------------------------------------------------------------------------------

F113 Video Duration
URI: https://photogrammetry.altervista.org/items/show/292 
Subclass of: E54_Dimension

Scope Note:
This class defines the duration of a video, measured in time (hours, minutes, seconds). The duration is an essential metric for understanding the length of content and its suitability for different contexts, such as teaching modules, presentations, or quick informational clips. Video duration can influence the viewer's engagement and is often constrained by platform requirements or project specifications. Expressed, where possible, with a Duration Data Type i.e. PT+numeral: H+numeral: M+ numeral: S (where H indicates hours, M indicates minutes, S indicates seconds.

Examples:

2 minutes and 34 seconds
1 hour and 15 minutes
30 seconds
 PT1H30M45S (for a video of 1 hour, 30 minutes and 45 seconds  for more info: https://www.w3schools.com/xml/schema_dtypes_date.asp 

Label: VideoRenderingDuration


—----------------------------------------------------------------------------------------

 
F114 AR/VR Project Description
URI: https://photogrammetry.altervista.org/items/show/293 
Subclass of: E62_String

Scope Note:
This class provides a detailed description of an AR/VR project, encompassing the project's objectives, key features, intended user experience, and any relevant background information. The description serves as an informative overview of the AR/VR project, summarizing its purpose and primary functionalities in a concise manner. It may also include technical specifications and usage contexts. Expressed, where possible, with a text string with a detailed description of the AR/VR project, its motivations and the technical aspects of the project.

Examples:

"An immersive VR experience for historical site exploration, enabling users to navigate and interact with reconstructions of ancient architecture."
"A collaborative AR application for educational purposes that visualizes complex scientific concepts in 3D."
Project BeaVir for Izumo Exhibition at the Archaeological museum of Izumo from 7/10/2022 to 4/12/2022

Label: ARVRProjectDescription
—----------------------------------------------------------------------------------------

F115 AR/VR Project Title/DOI
URI: https://photogrammetry.altervista.org/items/show/294 
Subclass of: E41_Appellation

Scope Note:
This class captures the title or DOI (Digital Object Identifier) of an AR/VR project. The title provides a recognizable name for the project, while the DOI serves as a unique identifier for accessing or referencing the project, especially for academic or research purposes. The presence of a DOI aids in the formal citation and retrieval of the project in digital repositories. Expressed, where possible, with a DOI URL of the article having the project as its subject or of the project itself, alternatively a text string reporting the identifying title of the project

Examples:

"Ancient Rome VR Experience"
"DOI: 10.1234/ar.vr.2024.001"
Label: ARVRProjectTitleDOI
—----------------------------------------------------------------------------------------

F116 AR/VR Project Category
URI: https://photogrammetry.altervista.org/items/show/295 
Subclass of: E55_Type

Scope Note:
This class defines the category of an AR/VR project, which classifies the project based on its primary function or domain of application. Categories may include educational, entertainment, simulation, or training purposes, providing context on the project's use case and target audience. Expressed, where possible, with a text string choosing from the following options:

Education and Training
Healthcare and Therapy
Cultural Heritage and Preservation
Entertainment and Gaming
Real Estate and Architecture
Retail and E-commerce
Tourism and Virtual Travel
Military and Defense
Marketing and Advertising
Industrial Design and Prototyping
Data Visualisation
Environmental Studies and Simulation
Art and Creative Expression
Social Interaction and Virtual Communities
Sports and Fitness
Event and Conference Management
Agriculture and Farming Technologies
Transportation and Navigation
Public Safety and Emergency Response
Accessibility and Assistive Technologies
Museum and Gallery Experiences
Fashion and Virtual Try-Ons
Urban Planning and Smart Cities
Performing Arts and Interactive Storytelling
Astronomy and Space Exploration


Examples:

Educational
Entertainment
Simulation
Training
Label: ARVRProjectCategory
—----------------------------------------------------------------------------------------

F117 AR/VR Project Platform
URI: https://photogrammetry.altervista.org/items/show/296 
Subclass of: D14_Software

Scope Note:
This class indicates the specific software platform or environment on which the AR/VR project is built or runs. Platforms may include dedicated AR/VR hardware systems, gaming engines, or software development environments. The platform can impact the compatibility, performance, and user experience of the AR/VR application. Expressed, where possible, with a text string indicating the specific type of platform used.

Examples:

Unity
Unreal Engine
Oculus Quest
Microsoft HoloLens
Label: ARVRProjectPlatform
—----------------------------------------------------------------------------------------
F118 AR/VR Project Real Coordinates
URI: https://photogrammetry.altervista.org/items/show/297 
Subclass of: E94_Space Primitive

Scope Note:
This class specifies the real-world coordinates used in an AR/VR project, which can be essential for geolocated or context-sensitive AR applications. These coordinates anchor virtual elements in specific real-world locations, enhancing the realism and situational relevance of AR experiences. Expressed, where possible, with coordinates expressed according to the principle
wgs84:lat + wgs84:long + geo:asWKT



Examples:

Latitude: 41.9028, Longitude: 12.4964 (Rome, Italy)
Latitude: 37.7749, Longitude: -122.4194 (San Francisco, CA)
example: wgs84:lat "45.0703"^^xsd:decimal ;
wgs84:long "7.6869"^^xsd:decimal ;
geo:asWKT "POINT(7.6869 45.0703)"^^geo:wktLiteral .

Label: ARVRProjectRealCoordinates
—----------------------------------------------------------------------------------------

F119 Mobile Application Operational System
URI: https://photogrammetry.altervista.org/items/show/298 
Subclass of: D14_Software

Scope Note:
This class defines the operational system on which a mobile application is designed to run. It includes details about compatibility with specific operating systems, which determines the application's usability across different devices and platforms.  Expressed, where possible, with a text string choosing from the following options:

Android
iOS
HarmonyOS
KaiOS
Sailfish OS
Windows Phone / Windows Mobile
BlackBerry OS
Symbian OS
Palm OS
Bada OS
Tizen OS
Ubuntu Touch
PostmarketOS
Replicant
LineageOS
Firefox OS
Plasma Mobile
e/OS


Examples:

iOS
Android
HarmonyOS
Windows Mobile
Label: MobileApplicationOperationalSystem
—----------------------------------------------------------------------------------------
F120 Programming Language
URI: https://photogrammetry.altervista.org/items/show/299 
Subclass of: E90_Symbolic Object

Scope Note:
This class indicates the programming language used to develop an application or project, which is crucial for understanding its technical foundation. Programming languages can affect the performance, flexibility, and maintainability of the codebase, and may be chosen based on project requirements or platform compatibility. 

Examples:

Python
JavaScript
C#
Swift
Label: ProgrammingLanguage
—----------------------------------------------------------------------------------------

F121 Educational Platform URL
URI: https://photogrammetry.altervista.org/items/show/300 
Subclass of: E42_Identifier

Scope Note:
This class provides the URL or web address of an educational platform where relevant resources, content, or tools can be accessed. This identifier is crucial for digital resources in the educational domain, allowing easy access to the platform and ensuring consistent referencing. Expressed, where possible, with URLs where the interactive project can be accessed.

Examples:

"https://www.khanacademy.org"
"https://www.coursera.org"
"https://www.edx.org"
https://vr.bearchaeo.unito.it/ 
  
Label: EducationalPlatformURL
—----------------------------------------------------------------------------------------




F122 Educational Platform Supported Browser
URI: https://photogrammetry.altervista.org/items/show/301 
Subclass of: D14_Software

Scope Note:
This class specifies the web browsers supported by an educational platform, which impacts accessibility and usability. Compatibility with certain browsers ensures a consistent user experience and helps avoid technical issues that may arise when using unsupported browsers. Expressed, where possible, with a text string choosing from the following options

Google Chrome
Mozilla Firefox
Safari
Microsoft Edge
Opera
Brave
Vivaldi
Microsoft Edge
Chromium
UC Browser
Tor Browser
Epiphany
Maxthon
Pale Moon
Waterfox
Midori
Lynx
QuteBrowser


Examples:

Google Chrome
Mozilla Firefox
Safari
Microsoft Edge

Label: EducationalPlatformSupportedBrowser

—----------------------------------------------------------------------------------------
F123 Educational Platform Server Web
URI: https://photogrammetry.altervista.org/items/show/302 
Subclass of: Physical Carrier

Scope Note:
This class denotes the specific web server on which the educational platform is hosted. Information about the server setup provides insights into the platform's infrastructure, reliability, and performance, as well as details about data security measures. Expressed, where possible, with a text string reporting the IP according to the IP format: xxx.xxx.x.x. 

Examples:

Apache HTTP Server
Nginx
Microsoft IIS
Amazon Web Services (AWS)
192.168.1.1 
Label: EducationalPlatformServerWeb
—----------------------------------------------------------------------------------------

F124 Printed Digital Twin Former Location
URI:https://photogrammetry.altervista.org/items/show/311 
Subclass of: E53_Place

Scope Note:
This class documents the former location of a printed digital twin, providing context about its provenance and previous usage. Such information is crucial for tracking the movement and historical context of 3D printed replicas, especially in cultural heritage and museum contexts.

Examples:

Exhibition Hall 3, National Museum of Archaeology
Storage Room, University of Cambridge Archaeology Department
Temporary Display at the Louvre Museum
Label: PrintedDigitalTwinFormerLocation
—---------------------------------------------------------------------------------------- 

F125 Interactive Project Description
URI: https://photogrammetry.altervista.org/items/show/312 
Subclass of: E62_String

Scope Note:
This class captures a detailed textual description of an interactive project, including its design, purpose, and features. This information is essential for understanding the nature of the project and its intended audience.

Examples:

An interactive touch-screen exhibit showcasing ancient Roman artifacts with 3D models and augmented reality overlays.
A virtual reality experience that allows users to explore a reconstructed medieval castle.
Label: InteractiveProjectDescription
—---------------------------------------------------------------------------------------- 

F126 Interactive Project Platform
URI: https://photogrammetry.altervista.org/items/show/313 
Subclass of: D14_Software

Scope Note:
This class defines the platform or software environment used to run an interactive project. The platform determines compatibility, performance, and accessibility of the project.

Examples:

Unity Engine
Unreal Engine
WebGL for browser-based interaction
ARKit for iOS
Label: InteractiveProjectPlatform
—---------------------------------------------------------------------------------------- 

F127 Interactive Project Former Location
URI: https://photogrammetry.altervista.org/items/show/314 
Subclass of: E53_Place

Scope Note:
This class identifies the former physical location where an interactive project was used, such as a multimedia station in a museum or an installation at an exhibition. Tracking former locations provides a historical record of the project's deployment and audience engagement.

Examples:

Interactive Kiosk at the British Museum's "Egyptian Mummies" Exhibit
Multimedia Station at the "Virtual Pompeii" Exhibition in Naples
Temporary Installation at the Smithsonian National Museum
Label: InteractiveProjectFormerLocation
—---------------------------------------------------------------------------------------- 

F128 Interactive Project Running Device
URI: https://photogrammetry.altervista.org/items/show/315 
Subclass of: D8_Digital Device

Scope Note:
This class specifies the device used to execute the interactive project. Knowing the running device is essential for understanding the technical requirements and constraints of the project.

Examples:

Microsoft HoloLens for an augmented reality application
Oculus Quest 2 for a virtual reality experience
Interactive touchscreen monitor for a multimedia kiosk
iPad Pro for a portable AR application

Label: InteractiveProjectRunningDevice
—---------------------------------------------------------------------------------------- 


F129 Database Table Schema and Structure
URI: https://photogrammetry.altervista.org/items/show/303 
Subclass of: E29_Design or Procedure

Scope Note:
This class describes the schema and structure of database tables, detailing the organization of data within the database. It includes table definitions, field names, data types, relationships between tables, and indexing strategies, which are critical for efficient data management and retrieval.

Examples:

Schema defining user data with fields: user_id, username, email, password_hash
Table structure with relationships for an inventory database including products, suppliers, and orders tables
Label: DatabaseTableSchemaAndStructure

—---------------------------------------------------------------------------------------- 
F130 Database Data Model
URI: https://photogrammetry.altervista.org/items/show/370 
Subclass of: D14_Software

Scope Note:
This class defines the data model used in the database, which determines how data is logically organized and how relationships between data entities are structured. The data model type affects data storage, retrieval efficiency, and the flexibility of the database.

Examples:

Relational model
Document-oriented model (e.g., MongoDB)
Graph model (e.g., Neo4j)
Key-value store
Label: DatabaseDataModel
—---------------------------------------------------------------------------------------- 

F131 GIS Reference System and Projection
URI: https://photogrammetry.altervista.org/items/show/305 
Subclass of: E29_Design or Procedure

Scope Note:
This class defines the geographic reference system and projection used in a GIS project, which establishes how spatial data is aligned on the earth's surface. Choosing an appropriate reference system and projection is essential for accurate spatial analysis and mapping.

Examples:

WGS84 (World Geodetic System 1984)
UTM Zone 33N
NAD83 (North American Datum 1983)
ETRS89 (European Terrestrial Reference System 1989)
Label: GISReferenceSystemAndProjection

—---------------------------------------------------------------------------------------- 
F132 GIS Bounding Box
URI: https://photogrammetry.altervista.org/items/show/306 
Subclass of: E94_Space Primitive

Scope Note:
This class represents the bounding box of a GIS dataset, defining the spatial extent of the data in terms of its minimum and maximum coordinates. The bounding box helps to limit the area of interest and manage data visualization and analysis within specified geographic boundaries.

Examples:

Min Longitude: -74.259, Min Latitude: 40.477, Max Longitude: -73.700, Max Latitude: 40.917 (Bounding box of New York City)
Min Longitude: 12.238, Min Latitude: 41.689, Max Longitude: 12.744, Max Latitude: 42.017 (Bounding box of Rome, Italy)
Label: GISBoundingBox
—---------------------------------------------------------------------------------------- 
 
F133 GIS Geospatial Data Format
URI: https://photogrammetry.altervista.org/items/show/307 
Subclass of: E90_Symbolic Object

Scope Note:
This class defines the data format of geospatial data used in a GIS project, which affects data interoperability, storage, and processing. The format determines how spatial data is encoded and read by GIS software.

Examples:

Shapefile (.shp)
GeoJSON (.geojson)
KML (Keyhole Markup Language)
TIFF (Tagged Image File Format for raster data)
Label: GISGeospatialDataFormat

—---------------------------------------------------------------------------------------- 
F134 Prospectus Legal Owner
URI: https://photogrammetry.altervista.org/items/show/308 
Subclass of: E39_Actor

Scope Note:
This class identifies the legal owner of a prospectus, usually an individual or organization with ownership rights over the document. Legal ownership information is important for establishing intellectual property rights and responsibilities.

Examples:

National Archaeological Museum
Smith Consulting Ltd.
Professor John Doe (individual researcher)
Label: ProspectusLegalOwner
—---------------------------------------------------------------------------------------- 

F135 Prospectus Former Location
URI: https://photogrammetry.altervista.org/items/show/309 
Subclass of: E53_Place

Scope Note:
This class documents the former location of a prospectus, which is relevant in cases where the document has been transferred or moved. Recording former locations can provide historical context for the document’s provenance and ownership history.

Examples:

University of Oxford Library Archives
Historical Records Office, Rome
Private Collection, Berlin
Label: ProspectusFormerLocation
—---------------------------------------------------------------------------------------- 

F136 CFD Project Title/DOI
URI: https://photogrammetry.altervista.org/items/show/310 
Subclass of: E41_Appellation

Scope Note:
This class captures the title or DOI (Digital Object Identifier) of a Computational Fluid Dynamics (CFD) project, providing a unique identifier for academic referencing and retrieval in digital databases. The title or DOI ensures that the CFD project can be properly cited and accessed.

Examples:

"Simulation of Airflow Around a Building Structure"
"DOI: 10.1000/cfd.project.2024.002"
Label: CFDProjectTitleDOI
—---------------------------------------------------------------------------------------- 


F137 Environmental Impact Studies Project Title/DOI
URI: https://photogrammetry.altervista.org/items/show/316 
Subclass of: E41_Appellation

Scope Note:
This class captures the title or DOI of a project focused on environmental impact studies. A title or DOI ensures that the project is uniquely identifiable and citable in academic or professional contexts.

Examples:

"Assessing the Environmental Impact of Urban Expansion in the Amazon Basin"
DOI: 10.1000/environmental.studies.2024.005
Label: EnvironmentalImpactStudiesProjectTitleDOI
—---------------------------------------------------------------------------------------- 
F138 S.U. Referenced Place of Excavation
URI: https://photogrammetry.altervista.org/items/show/317 
Subclass of: E53_Place

Scope Note:
This class identifies the specific location where the archaeological excavation took place, resulting in the recovery of the associated stratigraphic unit (S.U.). This information is critical for spatial and contextual analysis of archaeological findings.

Examples:

Site 24, Valley of the Kings, Egypt
Sector A, Pompeii, Italy
Layer 2, Göbekli Tepe, Turkey
Label: SUReferencedPlaceOfExcavation
—---------------------------------------------------------------------------------------- 

F139 S.U. Coordinates
URI: https://photogrammetry.altervista.org/items/show/318 
Subclass of: E94_Space Primitive

Scope Note:
This class specifies the precise spatial coordinates of a stratigraphic unit (S.U.) within an excavation site. These coordinates are essential for documenting the exact location of an archaeological find in three-dimensional space.

Examples:

Longitude: 31.235, Latitude: -22.745, Depth: 1.5m
X: 42.36, Y: 12.45, Z: -0.8 (local grid system)
Label: SUCoordinates
—---------------------------------------------------------------------------------------- 

F140 S.U. Material
URI:https://photogrammetry.altervista.org/items/show/319 
Subclass of: E57_Material

Scope Note:
This class describes the material composition of the stratigraphic unit (S.U.), which provides insight into the nature of the deposits and aids in determining the function or chronology of the context.

Examples:

Clay with small inclusions of limestone
Sandy silt with charcoal fragments
Burnt organic material mixed with pottery sherds
Label: SUMaterial

—------------------------------------------------------------------------------------------------------------
F141 Alignment
URI: https://photogrammetry.altervista.org/items/show/320 
Subclass of: F4_Modelling

Scope Note:
This class defines the process of aligning two spatial datasets, such as sparse point clouds, dense point clouds, 3D models, or any combination of these. Alignment is a fundamental step in 3D reconstruction and digital heritage workflows, ensuring that multiple datasets are spatially coherent and can be integrated into a single, unified representation. This process is essential for creating accurate and verifiable models, especially in contexts like cultural heritage, archaeology, and industrial design.

Examples:

The alignment of a sparse point cloud obtained via drone photogrammetry with a dense point cloud generated from terrestrial laser scanning for a castle façade reconstruction.
Aligning two dense point clouds of an archaeological artifact scanned using different devices (e.g., a photogrammetric model and a structured-light scanner model).
The registration of a dense point cloud with a 3D mesh generated through volumetric modeling for comparative analysis.
Aligning a historical 3D model reconstructed from archive photographs with a modern-day scan of the same object.

Label: Modelling_ModelAlignment

—-----------------------------------------------------------------------------------

F142 Comparison Activity of Different 3D Models
URI:https://photogrammetry.altervista.org/items/show/321 
Subclass of: E16 Measurement

Scope Note:
This class defines the activity of comparing two 3D models to assess their differences or similarities. The comparison could be based on various factors such as geometry, texture, scale, or resolution. It is typically used in contexts such as digital heritage, archaeology, and industrial design where precise and accurate models are critical. The input for this process often comes from digital twins or multiple 3D model datasets.

Examples:
A comparison of two 3D models of a historical sculpture to detect degradation or damage over time, with the use of a digital twin as the reference model.

Label: ComparisonActivity_3DModel
—-----------------------------------------------------------------------------------

F143 Tolerance Threshold Between Two 3D Models
URI: https://photogrammetry.altervista.org/items/show/322 
Subclass of: F142 Comparison Activity of Different 3D Models

Scope Note:
This class focuses on the threshold of tolerance between two 3D models, specifically quantifying the permissible deviation between them. It is important to determine the level of accuracy that is acceptable for the specific application, whether for quality assurance, restoration, or analysis. The tolerance threshold ensures that differences between models are within an acceptable range.

Examples:
Setting a tolerance threshold of 0.5 mm between two 3D models of a prehistoric tool to ensure that minor differences do not affect its usability in a digital restoration project.

Label: ToleranceThreshold_3DModels
—-----------------------------------------------------------------------------------

F144 Software Used for the Comparison of Two 3D Models
URI:https://photogrammetry.altervista.org/items/show/323 
Subclass of: D14 Software

Scope Note:
This class specifies the software tools used to perform the comparison between two 3D models. Different types of software can be used for various aspects of comparison, such as geometric alignment, texture mapping, or structural analysis. This class provides insights into the tools that support the evaluation of digital models.

Examples:
Using "CloudCompare" software to compare two 3D models of an ancient amphora to identify differences in surface geometry.

Label: SoftwareUsed_Comparison3DModels
—-----------------------------------------------------------------------------------

F145 Methodology Adopted for the Comparison
URI: https://photogrammetry.altervista.org/items/show/324 
Subclass of: E29 Design and Procedure

Scope Note:
This class describes the methodology or procedure used for the comparison of two 3D models. The methodology may include steps for pre-processing, alignment, tolerance measurement, and reporting of results. It provides the process framework for ensuring that the comparison is scientifically sound and meets the intended objectives.

Examples:
A step-by-step methodology for comparing 3D models of architectural ruins, including initial cleaning, alignment via software, surface comparison, and documentation of any significant deviations.

Label: Methodology_Comparison3DModels
—-----------------------------------------------------------------------------------

F146 Surface Detail Resolution
URI: https://photogrammetry.altervista.org/items/show/325 
Subclass of: E54 Dimension

Scope Note:
This class defines the resolution of the 3D model’s surface, typically expressed in microns or millimeters. It is crucial for capturing fine details of an object, especially when the 3D model is used for replication or for creating precise casts. The higher the resolution, the more detailed the representation of the surface features.

Examples:
The surface resolution of a 3D model of a Roman coin is set at 0.1 mm to capture all intricate engravings on its surface for accurate replication.

Label: SurfaceDetailResolution_3DModel
—-----------------------------------------------------------------------------------

F147 Material Tolerance Requirements
URI: https://photogrammetry.altervista.org/items/show/326 
Subclass of: E13 Attribute Assignment

Scope Note:
This class provides the material tolerance requirements during the printing or production process, specifying the acceptable margins of deviation. These requirements affect the precision and accuracy of the final replica, ensuring that it meets the desired specifications.

Examples:
For a 3D printed copy of an ancient vase, a material tolerance of ±0.2 mm is required to ensure a precise replication of the artifact's dimensions.

Label: MaterialToleranceRequirements_3DModel
—-----------------------------------------------------------------------------------

F148 Scaling Factor
URI: https://photogrammetry.altervista.org/items/show/327 
Subclass of: E13 Attribute Assignment

Scope Note:
This class specifies the scaling factor applied to the 3D model, whether it is at a 1:1 scale or modified for analysis or reproduction. The scaling factor ensures the model is properly adjusted to meet specific needs, whether it’s for physical reproduction, analysis, or restoration.

Examples:
A scaling factor of 1:5 is applied to the 3D model of a medieval sculpture for educational purposes, reducing its size while maintaining proportional accuracy.

Label: ScalingFactor_3DModel
—-----------------------------------------------------------------------------------

F149 Production Method Compatibility
URI:https://photogrammetry.altervista.org/items/show/328 
Subclass of: E29 Design and Procedure

Scope Note:
This class defines which production or printing technologies are compatible with the 3D model to ensure an accurate reproduction. Technologies could include SLA (Stereolithography), FDM (Fused Deposition Modeling), or resin printing, depending on the material and detail requirements of the replica.

Examples:
The 3D model of an ancient vase is compatible with SLA and resin printing technologies to achieve the level of surface detail necessary for museum display.

Label: ProductionMethodCompatibility_3DModel
—-----------------------------------------------------------------------------------

F150 Baseline Dataset Date
URI:https://photogrammetry.altervista.org/items/show/329 
Subclass of: E52 Time-Span

Scope Note:
This class specifies the date the original 3D model was created. It serves as the baseline reference for tracking changes over time, which is especially important in monitoring the condition of artifacts or digital preservation efforts.

Examples:
The baseline dataset date for the 3D model of a stone tablet is 2023-06-01, marking the start of digital preservation for the artifact.

Label: BaselineDatasetDate_3DModel
—-----------------------------------------------------------------------------------

F151 Surface Deviation Analysis Data
URI: https://photogrammetry.altervista.org/items/show/330 
Subclass of:  D11 Digital Measurement Event

Scope Note:
This class provides information on the surface deviation analysis of a 3D model compared to a previous reference model. It includes data on how much the current model deviates from the original, with a focus on dimensional accuracy and surface integrity.

Examples:
A surface deviation analysis of a 3D model of a statue, showing a 0.5 mm deviation in the nose area compared to the original.

Label: SurfaceDeviationAnalysis_3DModel
—-----------------------------------------------------------------------------------

F152 Restoration Intervention Metadata
URI: https://photogrammetry.altervista.org/items/show/331 
Subclass of: S18 Alteration

Scope Note:
This class describes any restoration interventions performed on an artifact, linked to the 3D model to document changes made during the restoration process. It helps track alterations and ensures a proper record of the restoration history.

Examples:
Metadata for the restoration of a 3D model of a fresco, which includes information on repainting efforts and structural repairs.

Label: RestorationInterventionMetadata_3DModel
—-----------------------------------------------------------------------------------
 PODS 1_2_38

F153 3D Model Spatial Metadata
URI: https://photogrammetry.altervista.org/items/show/332 
Subclass of: E13 Attribute Assignment

Scope Note:
This class represents a collection of spatial metadata associated with a 3D model, encompassing both technical and semantic aspects crucial for the description and management of 3D models in digital surveying contexts. It serves as a superclass for more specific subclasses that address georeferencing, orientation, model composition, and main face identification. This metadata is essential for ensuring the coherence, usability, and integration of 3D models in digital heritage workflows.

Examples:
Metadata describing the spatial orientation and georeferencing of a 3D model of an archaeological site to align it with a GIS map for analysis.

Label: Processing_SpatialMetadata
—-----------------------------------------------------------------------------------

F154 Georeferencing of the 3D Model
URI: https://photogrammetry.altervista.org/items/show/333 
Subclass of: F153 3D Model Spatial Metadata

Scope Note:
This class defines the georeferencing of a 3D model, which involves associating the model with a spatial or geographic coordinate system such as WGS84, UTM, or local systems. Georeferencing is critical for accurately placing the model in real-world space or aligning it with other geospatial data, such as maps or models from nearby areas.

Examples:
Georeferencing a 3D model of a historical monument to a UTM coordinate system to integrate it with topographic survey data.

Label: Georeferencing_3DModel
—-----------------------------------------------------------------------------------

F155 Orientation of the 3D Model
URI: https://photogrammetry.altervista.org/items/show/334 
Subclass of: F153 3D Model Spatial Metadata

Scope Note:
This class describes the orientation of a 3D model relative to a reference system, such as Cartesian axes (X, Y, Z). It includes information about the model’s rotation angles or the direction it faces in a global or local reference system. Accurate orientation metadata ensures consistency in analysis, visualization, and integration with other datasets.

Examples:
Documenting the orientation of a 3D model of a statue to align it with a global reference system for comparative analysis.

Label: Orientation_3DModel
—-----------------------------------------------------------------------------------

F156 Model Composition from Multiple Parts
URI: https://photogrammetry.altervista.org/items/show/335 
Subclass of: F153 3D Model Spatial Metadata

Scope Note:
This class refers to 3D models that are composed of multiple segments or parts rather than a single continuous object. For instance, the model may consist of various meshes that were initially captured separately and later aligned and merged into a single model during post-processing. It addresses scenarios where final assembly, such as mosaicking, has been completed. For initial alignment and registration of point clouds, refer to the class F104 Registration. Expressed with an integer numeral value

Examples:
A 3D model of an ancient temple composed of multiple meshes captured from different perspectives and later merged into a single, unified model.

Label: ModelComposition_MultipleParts
—-----------------------------------------------------------------------------------

F157 Identified Main Face
URI: https://photogrammetry.altervista.org/items/show/336 
Subclass of: F153 3D Model Spatial Metadata

Scope Note:
This class defines the identification of the "main face" of a 3D model, which serves as a reference during alignment or registration of various parts in the assembly process. For example, when registering multiple scans of an artifact, a stable or recognizable surface is often chosen as the primary reference for ensuring accurate alignment.

Examples:
Selecting the flat base of a 3D model of a ceramic vessel as the main face for aligning additional scans captured from other angles.

Label: MainFace_3DModel
—-----------------------------------------------------------------------------------

F158 Mesh Density and Uniformity
URI: https://photogrammetry.altervista.org/items/show/338 
Subclass of: E54 Dimension

Scope Note:
This class defines the density and uniformity of the mesh used in the 3D model. It is critical for ensuring that the mesh has sufficient resolution and consistency to perform accurate structural load simulations or other types of analysis. A uniform and sufficiently dense mesh allows for precise data modeling, especially when conducting simulations for engineering, architectural, or restoration purposes.

Examples:
A 3D model of a building's façade used for structural analysis requires a mesh density of 2mm to ensure accurate force distribution simulations in software. The uniformity of the mesh ensures that no weak points distort the results.

Label: MeshDensity_3DModel
—-----------------------------------------------------------------------------------

F159 Material Properties Assignment
URI: https://photogrammetry.altervista.org/items/show/339 
Subclass of: S4 Observation

Scope Note:
This class provides information about the material properties assigned to a 3D model, such as density, elastic modulus, and compressive strength. These properties are vital for conducting simulations like structural analysis or load-bearing evaluations, as they define how the material behaves under different conditions and forces. The proper assignment of material properties ensures the realism and accuracy of virtual simulations.

Examples:
Assigning steel with a density of 7850 kg/m³, an elastic modulus of 200 GPa, and a compressive strength of 250 MPa to a 3D model of a bridge component used in a stress test simulation.

Label: MaterialProperties_3DModel
—-----------------------------------------------------------------------------------

F160 Boundary Conditions and Constraints
URI: https://photogrammetry.altervista.org/items/show/340 
Subclass of: E3 Condition State

Scope Note:
This class defines the boundary conditions and constraints applied to a 3D model for simulations. Boundary conditions specify how the model interacts with the environment (e.g., fixed supports or loading conditions), while constraints define the limitations or restrictions in movement or deformation. Both are essential for accurately simulating real-world behavior during structural or physical analysis.

Examples:
In a simulation of a 3D model of a bridge, boundary conditions might specify that one end is fixed (cannot move), and forces are applied at specific points to simulate traffic load. Constraints may limit how much displacement is allowed at the bridge’s joints.

Label: BoundaryConditions_3DModel
—-----------------------------------------------------------------------------------

F161 Finite Element Analysis (FEA) Model Integration
URI: [insert URI here]
Subclass of: S21 Measurement

Scope Note:
This class describes the integration of the 3D model with Finite Element Analysis (FEA) tools. FEA is a computational method used to predict how a model will respond to physical forces, vibrations, heat, or other physical effects by breaking the model into smaller, manageable parts (finite elements). This class stores the necessary data for linking the 3D model with FEA software and the parameters used for the simulation.

Examples:
A 3D model of a bridge undergoes integration with FEA software where the model is divided into smaller elements, and parameters like stress, strain, and displacement are set to simulate the bridge's response to traffic loads.

Label: FEAIntegration_3DModel

—-----------------------------------------------------------------------------------


F162 Structural Load Parameters
URI: https://photogrammetry.altervista.org/items/show/342 
Subclass of: E62 String

Scope Note:
This class contains detailed information about the types of loads applied to a 3D model, such as static, dynamic, or distributed loads, along with the corresponding units of measurement. These parameters are essential for performing structural analysis, ensuring that the model can accurately simulate real-world stresses and forces. The specification of load types and units is crucial for ensuring that simulations yield realistic and reliable results for engineering or architectural applications.

Examples:
For a 3D model of a building, static loads might include the weight of the structure itself, while dynamic loads could include wind forces or traffic impacts. The units for these loads might be expressed in Newtons (N) or kilonewtons (kN).

Label: StructuralLoadParameters_3DModel
—-----------------------------------------------------------------------------------

F163 Modelling Phase
URI: https://photogrammetry.altervista.org/items/show/343 
Subclass of: F101 Survey Phase

Scope Note:
This class defines the set of instructions related to the modeling phase of the 3D model creation process. The modeling phase includes all steps and guidelines followed during the transformation of raw data into a digital 3D model, such as geometric shaping, data processing, and initial refinement. This phase is critical for ensuring that the 3D model represents the desired object or structure with accuracy and fidelity.

Examples:
In the modeling phase for a 3D replica of an archaeological artifact, the process may involve converting scan data into a solid mesh and cleaning up any errors in the raw data to ensure that the final model is precise and usable for analysis or printing.

Label: ModellingPhase
—-----------------------------------------------------------------------------------

F164 Exporting Phase
URI:https://photogrammetry.altervista.org/items/show/344 
Subclass of: F101 Survey Phase

Scope Note:
This class describes the set of instructions related to the final export phase of the 3D model. The exporting phase includes all steps and formats used to output the model for different applications, such as printing, virtual visualization, or further analysis. It ensures the model is compatible with target platforms or devices and meets specific technical requirements for export.

Examples:
After the modeling of an architectural structure, the exporting phase might include converting the 3D model into a format suitable for 3D printing, such as STL, or for use in a VR environment, such as FBX.

Label: ExportingPhase
—-----------------------------------------------------------------------------------

F166 Mobile Application Implementation
URI:https://photogrammetry.altervista.org/items/show/345 
Subclass of: F5 Exporting

Scope Note:
This class refers to the activity of uploading or implementing a 3D model on a mobile application. This phase involves integrating the model into an interactive mobile platform, allowing users to view, interact with, or manipulate the 3D model via their mobile devices. This is especially important for applications in digital heritage, e-commerce, or virtual tourism.

Examples:
Uploading a 3D model of an ancient statue to a mobile application where users can explore the object interactively by rotating, zooming, or analyzing it in mobile application.

Label: Exporting_MobileApplicationImplementation
—-----------------------------------------------------------------------------------

F167 Interactive Application
URI:https://photogrammetry.altervista.org/items/show/346 
Subclass of: D14 Software

Scope Note:
This class refers to software applications that allow users to interact with 3D models, often in real-time. These applications are used to visualize models, conduct analyses, or explore virtual environments. Interactive applications are common in fields like virtual museums, educational software, and gaming, where user engagement is critical for experiencing the 3D model in context.

Examples:
A virtual museum application where users can explore 3D models of archaeological artifacts, view them from different angles, and access information about each object. Another example could be a game where players interact with realistic 3D models of vehicles or environments.

Label: InteractiveApplication_Software
—-----------------------------------------------------------------------------------

F165 Registration Activity 
URI: https://photogrammetry.altervista.org/items/show/347 
subclass of: F47 Densification 

Scope Note
The F165 Registration Activity class refers to the process of aligning and merging multiple point clouds or 3D models into a single, coherent model. This class captures the concept of registration, a key step in photogrammetry and 3D reconstruction workflows where data collected from different viewpoints or sources is combined to create a comprehensive representation of an object or scene.
In this process, registration involves the precise alignment of overlapping regions of point clouds or 3D models, ensuring that they share a common coordinate system and that the surfaces match accurately. This can be done manually or, more commonly, through automated algorithms that minimize alignment errors by detecting corresponding points or features across the datasets.
Registration is an essential step, especially when working with large datasets or complex scenes that require the integration of multiple scans. This class describes the methodology and actions taken to perform the registration, including the matching of common features, alignment algorithms used, and optimization techniques to reduce errors.
F165 is a subclass of F47 Densification, as registration often begins with individual densified point clouds—highly detailed datasets representing surfaces—which are then combined into a unified model for further processing or analysis.

Examples:

The registration (F165) of two overlapping point clouds from different vantage points was performed to generate a complete 3D model of an ancient temple.
During the photogrammetric survey of a large site, registration (F165) was used to merge multiple 3D models captured from different sections, resulting in a unified representation of the site.
Automated registration (F165) was applied to fuse point clouds captured from aerial and ground-based photogrammetry, creating a comprehensive 3D model for analysis.

Label: RegistrationActivity

—-----------------------------------------------------------------------------------


New properties declaration 1_2_39 

Y96: has produced aligned digital object
URI: https://photogrammetry.altervista.org/items/show/348 
Subproperty of: None
Domain: F141 Alignment
Range: F104 Registration (Fusion of Multiple Point Clouds or 3D Models)
Scope Note:
This property connects the Alignment process (F141) with the resultant fused 3D model or point cloud, signifying that the alignment procedure has produced an aligned digital object. It indicates that the aligned data, typically from multiple sources or viewpoints, has been merged into a unified model, facilitating further analysis or visualization.
Examples:
The alignment process (F141) has produced an aligned digital object (F104) by combining multiple point clouds of a monument captured from different perspectives.
A series of LiDAR scans underwent alignment (F141), resulting in a complete, unified 3D model of a landscape (F104).
Label: has_produced_aligned_digital_object

Y97: has processing description
URI: https://photogrammetry.altervista.org/items/show/349 
Subproperty of: P3 has note
Domain: F3 Processing
Range: F110 Processing Description
Scope Note:
This property links the Processing class (F3) with a detailed description of the processing steps or methodologies applied. It indicates that the specific processing procedure for the digital data has been documented in the associated processing description, typically capturing the workflow, tools, and techniques used.
Examples:
The 3D scan data processing (F3) has processing description (F110) that includes the photogrammetric techniques and software used to generate the 3D model.
The processing description (F110) details the algorithms and settings applied during the conversion of raw point cloud data (F3) into a final 3D mesh.
Label: has_processing_description

Y98: has video resolution
URI: https://photogrammetry.altervista.org/items/show/350 
Subproperty of: P40 observed dimension
Domain: F75 Project Video
Range: F112 Video Resolution
Scope Note:
This property connects a video project (F75) with its resolution (F112), indicating the level of detail in the video captured during the project. It provides information about the resolution of the video content, crucial for understanding the clarity and quality of visual information in the context of the project.
Examples:
The project video (F75) has video resolution (F112) of 4K, ensuring high-definition quality for visual analysis of the archaeological excavation.
The video resolution (F112) for the documentary project (F75) was set to 1080p for optimal viewing on standard display devices.
Label: has_video_resolution

Y99: has video duration
URI: https://photogrammetry.altervista.org/items/show/351 
Subproperty of: P40 observed dimension
Domain: F75 Project Video
Range: F113 Video Duration
Scope Note:
This property links a video project (F75) to its duration (F113), defining the total length of the video. It is important for understanding the time span of the recorded content, which can be significant when analyzing the progression of a process or the coverage of an event.
Examples:
The project video (F75) has video duration (F113) of 45 minutes, covering an entire survey process from start to finish.
A short time-lapse video documenting the excavation process (F75) has video duration (F113) of 5 minutes.
Label: has_video_duration

Y100: use AR/VR project description
URI: https://photogrammetry.altervista.org/items/show/352 
Subproperty of: P3 has note
Domain: F98 AR/MR Project Implementation
Range: F114 AR/VR Project Description
Scope Note:
This property connects the Augmented Reality or Mixed Reality Project Implementation (F98) with the associated AR/VR Project Description (F114). It describes the details of how augmented reality or virtual reality was used in the project, outlining the technological implementation and the intended purpose of the AR/VR experience.
Examples:
The AR/MR project implementation (F98) uses AR/VR project description (F114) to explain the interactive virtual tour created for visitors to explore the archaeological site.
The AR/VR project description (F114) outlines the setup for using VR to simulate historical reconstructions in the context of the museum exhibit (F98).
Label: use_AR_VR_project_description
—-------------------------------------------------------------------------------------------------------

Y101: use project identifier
URI:https://photogrammetry.altervista.org/items/show/353 
Subproperty of: P3 has note
Domain: F98 AR/MR Project Implementation
Range: F115 AR/VR Project Title/DOI
Scope Note:
This property connects an AR/MR Project Implementation (F98) with a unique project identifier (F115), typically represented by a title or DOI (Digital Object Identifier). It indicates that a specific identifier has been assigned to the project, which can be used to reference or access the project within a broader digital or academic context.
Examples:
The AR/MR project implementation (F98) uses project identifier (F115) for the unique DOI assigned to a scholarly article describing the project.
The project identifier (F115) is a standardized code used to catalog the AR/VR experience in a global digital archive.
Label: use_project_identifier

Y102: use project category
URI: https://photogrammetry.altervista.org/items/show/354 
Subproperty of: P2 has type
Domain: F98 AR/MR Project Implementation
Range: F116 AR/VR Project Category
Scope Note:
This property connects the AR/MR Project Implementation (F98) with its category (F116), specifying the type or classification of the AR/VR project. It indicates that the project has been categorized under a specific genre, such as education, entertainment, cultural heritage, or research, which helps contextualize its purpose and content.
Examples:
The AR/MR project implementation (F98) uses project category (F116) to define the project as an educational tool for teaching history.
The project category (F116) for the AR/VR project is set to "Cultural Heritage," describing an immersive tour through historical monuments.
Label: use_project_category

Y103: use project AR/VR platform
URI:https://photogrammetry.altervista.org/items/show/355 
Subproperty of: P16 used specific object
Domain: F98 AR/MR Project Implementation
Range: F117 AR/VR Project Platform
Scope Note:
This property connects an AR/MR Project Implementation (F98) with the specific AR/VR platform (F117) used to deploy or support the project. It signifies that the project is designed for a particular AR/VR platform, such as Oculus, HTC Vive, or mobile AR platforms like ARKit or ARCore.
Examples:
The AR/MR project implementation (F98) uses the AR/VR platform (F117) of HTC Vive for an immersive virtual experience in an art gallery.
The AR/VR platform (F117) used for the educational AR/MR project is based on the mobile ARKit platform for iOS devices.
Label: use_project_AR_VR_platform

Y104: use AR/VR real coordinates
URI: https://photogrammetry.altervista.org/items/show/356 
Subproperty of: P169 defines spacetime volume
Domain: F98 AR/MR Project Implementation
Range: F118 AR/VR Project Real Coordinates
Scope Note:
This property connects an AR/MR Project Implementation (F98) with its real-world spatial coordinates (F118). It specifies that the AR/VR project makes use of actual geographic or physical coordinates to place digital content accurately within the real world, such as in augmented reality applications where virtual objects interact with real-world locations.
Examples:
The AR/MR project implementation (F98) uses AR/VR real coordinates (F118) to anchor digital models within the actual coordinates of an archaeological site.
The project uses AR/VR real coordinates (F118) to align virtual furniture placements with real-world dimensions in an interior design AR app.
Label: use_AR_VR_real_coordinates

Y105: use mobile OS
URI: https://photogrammetry.altervista.org/items/show/357 
Subproperty of: P16 used specific object
Domain: F166 Mobile Application Implementation
Range: F119 Mobile Application Operational System
Scope Note:
This property connects a Mobile Application Implementation (F166) with the mobile operating system (F119) on which the application runs. It specifies the operating system (OS) used, such as iOS or Android, which determines the compatibility and features of the mobile application.
Examples:
The mobile application implementation (F166) uses mobile OS (F119) Android for delivering an interactive AR experience in a museum.
The AR-based mobile app for an art gallery (F166) uses mobile OS (F119) iOS to run on iPhones and iPads.
Label: use_mobile_OS

Y106: use programming language
URI: https://photogrammetry.altervista.org/items/show/358 
Subproperty of: P33 use specific technique
Domain: F166 Mobile Application Implementation
Range: F120 Programming Language
Scope Note:
This property connects a Mobile Application Implementation (F166) with the programming language (F120) used to develop the application. It indicates the specific software development language, such as Java, Swift, or C#, used to code the mobile application for the AR/MR project.
Examples:
The mobile application implementation (F166) uses programming language (F120) Swift for developing an iOS-based AR app for architecture visualization.
The AR/VR mobile app (F166) is built using programming language (F120) Unity C# for cross-platform compatibility on both Android and iOS.
Label: use_programming_language
—--------------------------------------------------------------------------------------

Y107: has platform URL
URI: [Insert URI here]
Subproperty of: P3 has note
Domain: F92 Interactive Project Implementation
Range: F121 Educational Platform URL
Scope Note:
This property connects an Interactive Project Implementation (F92) with the platform URL (F121), which provides the link to the educational platform hosting the interactive project. It represents the web address of the platform where users can access and interact with the AR/VR or digital content.
Examples:
The interactive project implementation (F92) has a platform URL (F121) leading to the online educational portal where students can engage with the virtual learning resources.
The project (F92) has a platform URL (F121) for an online interactive platform, allowing learners to explore 3D models of historical artifacts.
Label: has_platform_URL

Y108: is supported in browser
URI: https://photogrammetry.altervista.org/items/show/360 
Not a Subproperty
Domain: F92 Interactive Project Implementation
Range: F122 Educational Platform supported browser
Scope Note:
This property indicates whether the interactive project (F92) is supported by specific web browsers (F122). It highlights the browser compatibility of an educational platform, specifying which web browsers can be used to access and run the interactive content.
Examples:
The interactive project implementation (F92) is supported in browsers (F122) such as Google Chrome, Mozilla Firefox, and Safari for seamless user experience.
The project (F92) is compatible with browsers (F122) like Edge and Opera, ensuring access across various web platforms.
Label: is_supported_in_browser

Y109: is carried in web server
URI:https://photogrammetry.altervista.org/items/show/361 
Subproperty of: L19i is stored on
Domain: F167 Interactive Application
Range: F123 Educational Platform Server Web
Scope Note:
This property connects an Interactive Application (F167) with the web server (F123) where the platform or content is hosted. It specifies that the educational interactive application is stored and served from a particular web server, ensuring that it is accessible through a web interface.
Examples:
The interactive application (F167) is carried on a web server (F123) providing access to online educational content via a central server.
The educational platform’s content (F167) is hosted on a web server (F123), ensuring that users can access the application via web browsers.
Label: is_carried_in_web_server

Y110: has db structure
URI: https://photogrammetry.altervista.org/items/show/362 
Subproperty of: P33 use specific technique
Domain: F95 Database Project Implementation
Range: F129 DatabaseTable Schema and Structure
Scope Note:
This property connects a Database Project Implementation (F95) with the database structure (F129), describing the design and schema of the database tables used to store and manage the data for the project. It defines the structure that organizes data within the database, such as tables, fields, and relationships.
Examples:
The database project implementation (F95) has a db structure (F129) which organizes information into tables for storing user data and project results.
The database schema (F129) for the project (F95) includes tables for storing metadata, 3D model properties, and user interactions.
Label: has_db_structure

Y111: has db model
URI: https://photogrammetry.altervista.org/items/show/363 
Subproperty of: P16 used specific object 
Domain: F95 Database Project Implementation
Range: F130 Database Data Model
Scope Note:
	This property links a Database Project Implementation (F95) with the data model (F130), which represents the conceptual structure of the data. It details how the data is stored, processed, and related within the database system, defining the logical structure of the data entities and their relationships.
Examples:
The database project implementation (F95) has a db model (F130) that defines entities such as users, projects, and interactions in the educational system.
The data model (F130) for the database (F95) organizes and connects tables for tracking metadata and project files in a cloud-based system.
Label: has_db_model

—---------------------------------------------------------------
Y112: has GIS reference system
URI: https://photogrammetry.altervista.org/items/show/364 
Subproperty of: none
Domain: F82 Reference GIS System
Range: F131 GIS reference system and projection
Scope Note:
	This property links a Reference GIS System (F82) with a GIS reference system and projection (F131), specifying the spatial reference system used for mapping and geospatial data analysis. It defines the projection and coordinate system that allows geospatial data to be accurately positioned within a global or local context.
Examples:
The Reference GIS System (F82) has a GIS reference system and projection (F131), such as WGS84, used for mapping archaeological site locations.
The GIS reference system (F131) and projection, like UTM Zone 33N, are linked to the reference GIS system (F82) to ensure precise geospatial data analysis.
Label: has_GIS_reference_system

Y113: has GIS bounding box
URI: https://photogrammetry.altervista.org/items/show/365 
Subproperty of: none
Domain: F82 Reference GIS System
Range: F132 GIS Bounding Box
Scope Note:
This property connects a Reference GIS System (F82) with a GIS Bounding Box (F132), representing the geographic extent or boundary of the geospatial data. It defines the minimum and maximum coordinates that describe the rectangular area in which the geospatial data resides.
Examples:
The Reference GIS System (F82) has a GIS bounding box (F132), which delineates the spatial extent of the archaeological site mapped in the GIS.
The GIS bounding box (F132) for the area of interest includes coordinates ranging from 40°N to 42°N latitude and 12°E to 14°E longitude.
Label: has_GIS_bounding_box

Y114: has geospatial data format
URI: https://photogrammetry.altervista.org/items/show/366 
Subproperty of: none
Domain: F82 Reference GIS System
Range: F133 GIS Geospatial Data Format
Scope Note:
This property connects a Reference GIS System (F82) with a GIS Geospatial Data Format (F133), specifying the file format or structure used to store and exchange geospatial data. It indicates the format in which the GIS data is represented, ensuring compatibility with various GIS software and tools.
Examples:
The Reference GIS System (F82) uses a GIS geospatial data format (F133) such as GeoTIFF for raster data or Shapefile for vector data.
The GIS geospatial data format (F133) for the project includes KML files used to represent geospatial coordinates and features in Google Earth.
Label: has_geospatial_data_format

Y115: has legal owner of the prospectus
URI: https://photogrammetry.altervista.org/items/show/367 
Subproperty of: P105 right held by
Domain: F87 3D Model Prospectus
Range: F134 Prospectus Legal Owner
Scope Note:
	This property links a 3D Model Prospectus (F87) with the Prospectus Legal Owner (F134), identifying the legal entity or individual that owns the rights to the 3D model or its associated documentation. It ensures proper attribution and protection of intellectual property related to the 3D model.
Examples:
The 3D model prospectus (F87) has a legal owner (F134), such as a museum or research institution that holds the copyright for the virtual reconstruction.
The legal owner (F134) of the prospectus (F87) is the university department responsible for the 3D modeling project.
Label: has_legal_owner_of_the_prospectus

Y116: has legal and former location archiving
URI: https://photogrammetry.altervista.org/items/show/368 
Subproperty of: none
Domain: F87 3D Model Prospectus
Range: F135 Prospectus Former Location
Scope Note:
This property connects a 3D Model Prospectus (F87) with the Prospectus Former Location (F135), specifying the previous geographical location or archive where the 3D model or related artifacts were originally found, recorded, or stored.
Examples:
The 3D model prospectus (F87) has a legal and former location archiving (F135) in a specific archaeological site in Italy where the artifact was originally discovered.
The prospectus (F87) notes the former location (F135) where the 3D model was archived before being digitized and stored in the current system.
Label: has_legal_and_former_location_archiviation

Y117: has CFD project identifier
URI: https://photogrammetry.altervista.org/items/show/369 
Subproperty of: P1 is identified by 
Domain: F89 Project Analysis
Range: F136 CFD Project Title/DOI
Scope Note:
This property connects a Project Analysis (F89) with a CFD Project Title/DOI (F136), linking the project with its computational fluid dynamics (CFD) analysis identifier. This ensures that each CFD analysis is properly cited and referenced, including project titles or DOIs for academic or professional use.
Examples:
The project analysis (F89) has a CFD project identifier (F136), linking it to the CFD model used to simulate airflow in an architectural space.
The CFD project identifier (F136) for the analysis (F89) includes the DOI of a publication that describes the computational fluid dynamics simulation.
Label: has_CFD_project_identifier

Y118: has video format type
URI: https://photogrammetry.altervista.org/items/show/377 
Subproperty of: P2 has type 
Domain: F75 Project Video
Range: F111 Video Format Type
Scope Note:
	This property connects a Project Video (F75) with a Video Format Type (F111), specifying the type of video file format used for storing and displaying the project’s video content. It ensures compatibility with video playback systems and software.
Examples:
The project video (F75) has a video format type (F111), such as MP4, for easy integration into the online educational platform.
The video format type (F111) for the project video (F75) is AVI, suitable for high-definition video presentations.
Label: has_video_format_type

Y119: has type of acquisition environment
URI:https://photogrammetry.altervista.org/items/show/378 
Subproperty of: P2 has type 
Domain: F42 Place of Acquisition
Range: F170 Acquisition environment type
Scope Note:
	This property links a Place of Acquisition (F42) with an Acquisition Environment Type (F166), specifying the environmental conditions or setup under which data was captured. This could include settings such as indoor, outdoor, laboratory, or field-based environments that affect the acquisition process.
Examples:
The place of acquisition (F42) has a type of acquisition environment (F170), such as an indoor lab setup used for scanning artifacts.
The acquisition environment type (F166) for the field survey project (F42) was an outdoor archaeological excavation site, with measurements taken in natural lighting conditions.
Label: has_type_of_acquisition_environment


Y120: has point cloud input for processing
URI: https://photogrammetry.altervista.org/items/show/379 
Subproperty of: L10 had input
Domain: F26 Point Cloud
Range: F47 Densification
Scope Note:
	This property links a Point Cloud (F26) with the process of Densification (F47). It specifies that the point cloud, as an initial input, undergoes densification to enhance the resolution and accuracy of the data. Densification increases the number of points in the point cloud, making it more detailed and suitable for further processing, such as 3D modeling or analysis.
Examples:
The Point Cloud (F26) collected from the site has point cloud input for processing (F47), which was used to generate a high-density model for architectural restoration.
A low-resolution point cloud (F26) was fed into the densification process (F47) to create a detailed 3D model of a cultural heritage artifact.
Label: has_point_cloud_input_for_processing

Y121: has 3D Model Spatial Metadata
URI: https://photogrammetry.altervista.org/items/show/380 
Subproperty of: P15i influenced
Domain: F100 Digital Twin
Range: F153 3D Model Spatial Metadata
Scope Note:
	This property connects a Digital Twin (F100) with 3D Model Spatial Metadata (F153), specifying that the digital twin includes the metadata detailing the spatial characteristics of the 3D model. The metadata may include information on scale, dimensions, coordinate systems, or transformations that are vital for ensuring accurate placement and interaction within a real-world context.
Examples:
The Digital Twin (F100) has 3D Model Spatial Metadata (F153), which defines the scale and coordinate system used in the digital reconstruction of the building.
The 3D Model Spatial Metadata (F153) in the Digital Twin (F100) includes the geospatial data required to align the virtual model with real-world coordinates.
Label: has_3D_model_spatial_metadata

Y122: was influenced by eidotype
URI:https://photogrammetry.altervista.org/items/show/381 
Subproperty of: P15 was influenced by
Domain: F2 Acquisition
Range: F40 Eidotype
Scope Note:
	This property links the Acquisition (F2) process with an Eidotype (F40), indicating that the acquisition was influenced or guided by the eidotype. An eidotype refers to an idealized or conceptual representation, such as a blueprint or reference model, which informs the acquisition process by providing a visual or theoretical guide for capturing the data.
Examples:
The Acquisition (F2) of the archaeological site was influenced by an Eidotype (F40) that depicted a historical reconstruction of the site.
The 3D scan (F2) of the ancient sculpture was influenced by the Eidotype (F40), which showed a conceptual reconstruction based on previous research.
Label: was_influenced_by_eidotype

Y123: has exporting description
URI: https://photogrammetry.altervista.org/items/show/382 
Subproperty of: P3 has note
Domain: F5 Exporting
Range: F69 Exporting Description
Scope Note:
	This property links an Exporting (F5) activity with an Exporting Description (F69), providing a detailed account of the export process. This description typically includes technical specifications, such as file formats, data compression methods, or software used for exporting the data, ensuring that the exported file is usable for its intended purposes.
Examples:
The Exporting (F5) of the 3D model was accompanied by an Exporting Description (F69) that outlined the use of the OBJ file format for digital preservation.
The Exporting Description (F69) for the digital asset included details on the compression methods used to reduce file size without compromising quality.
Label: has_exporting_description

Y124: was continued by subsequent digital machine event
URI: https://photogrammetry.altervista.org/items/show/383 
Subproperty of: P134 continued
Domain: D7 Digital Machine Event
Range: D7 Digital Machine Event
Scope Note:
	This property connects one Digital Machine Event (D7) to another subsequent Digital Machine Event (D7), indicating a continuation in the sequence of events related to digital processing or modeling. It is used to represent the flow from one stage of digital activity to another, such as from data acquisition to processing or modeling, ensuring a coherent workflow for the entire digital project.
Examples:
The initial Digital Machine Event (D7), involving data acquisition, was continued by a subsequent Digital Machine Event (D7) focused on the 3D modeling process.
A series of Digital Machine Events (D7) were initiated with data acquisition and later continued by modeling, followed by export to a digital platform.
Label: was_continued_by_subsequent_digital_machine_event

Y125: used Modelling Phase instruction
URI: https://photogrammetry.altervista.org/items/show/384 
Subproperty of: P33 used specific technique
Domain: F4 Modelling
Range: F163 Modelling Phase
Scope Note:
	This property links a Modelling (F4) process to a Modelling Phase (F163), indicating that the modeling was guided or structured by specific instructions or methodologies outlined during the Modelling Phase. This phase may include techniques or instructions on how to create or refine a 3D model, helping to ensure consistency and accuracy across different modeling tasks.
Examples:
The 3D modeling (F4) process used specific instructions from the Modelling Phase (F163), which outlined the steps for creating a detailed model of a historical artifact.
During the Modelling Phase (F163), specific techniques were employed to improve the precision of the 3D model by incorporating feedback from experts.
Label: used_modelling_phase_instruction
—--------------------------------------------------------

Y126: used Exporting Phase Instruction
URI: https://photogrammetry.altervista.org/items/show/385 
Subproperty of: P33 used specific technique
Domain: F5 Exporting
Range: F164 Exporting Phase
Scope Note:
	This property connects an Exporting (F5) activity with specific instructions or methodologies outlined during the Exporting Phase (F164). It indicates that the exporting process followed a structured set of instructions designed to ensure that the digital data or models are exported correctly and in the desired formats for further use, analysis, or sharing. These instructions may include file formats, compression methods, and data handling protocols.
Examples:
The Exporting (F5) process used specific instructions from the Exporting Phase (F164), which included the export of a 3D model in both OBJ and STL formats for printing.
During the Exporting Phase (F164), the instructions were followed to convert the model into a VR-compatible file format for use in a virtual museum.
Label: used_exporting_phase_instruction

Y127: has produced registered point cloud
URI: https://photogrammetry.altervista.org/items/show/386 
Subproperty of: L11 had output
Domain: F165 Registration Activity
Range: F104 Registration (registered point cloud)
Scope Note:
	This property links a Registration Activity (F165) to the resulting Registered Point Cloud (F104). It indicates that the registration process has been completed and a point cloud, now aligned and merged from multiple scans, has been produced. This registered point cloud serves as a unified, coherent dataset ready for further analysis, 3D modeling, or visualization.
Examples:
The Registration Activity (F165) was successful and has produced a registered point cloud (F104), enabling a detailed 3D model of the archaeological site.
After performing the registration of multiple scans, the registration activity (F165) produced a registered point cloud (F104) for further processing in architectural design.
Label: has_produced_registered_point_cloud

Y128: was analyzed with
URI:https://photogrammetry.altervista.org/items/show/387 
Subproperty of: O24 measured
Domain: F88 3D Model for Research
Range: F105 Interrogation Tools
Scope Note:
	This property indicates that a 3D model (F88) has been analyzed using specific interrogation tools (F105). These tools are designed to extract, measure, or manipulate the 3D data for research purposes. The analysis can involve measuring distances, examining surface properties, or simulating real-world conditions within the model.
Examples:
The 3D Model for Research (F88) was analyzed with interrogation tools (F105) to measure the structural integrity of a historical building.
The digital twin (F100) was analyzed with F105 Interrogation Tools, which allowed researchers to simulate environmental conditions affecting the model.
Label: was_analyzed_with

Y129: has acquisition location type
URI: https://photogrammetry.altervista.org/items/show/388 
Subproperty of: P2 has type
Domain: F2 Acquisition
Range: F106 Acquisition Location Type
Scope Note:
	This property links an Acquisition event (F2) to the specific type of acquisition location (F106), detailing where the data was collected. The acquisition location type could refer to different environments, such as outdoor fieldwork, laboratory settings, or virtual environments, providing context for the data collection process.
Examples:
The Acquisition (F2) of the cultural heritage artifact was conducted in an outdoor archaeological site and was classified under an Acquisition Location Type (F106) as a field location.
The Acquisition (F2) in the lab was carried out in a controlled environment, with the Acquisition Location Type (F106) defined as a laboratory.
Label: has_acquisition_location_type

Y130: was influenced by calibration instrument
URI:https://photogrammetry.altervista.org/items/show/389 
Subproperty of: P15 was influenced by
Domain: F2 Acquisition
Range: F108 Calibration of the instrument
Scope Note:
	This property connects the Acquisition (F2) event with the Calibration of the instrument (F108), indicating that the acquisition process was influenced or guided by the calibration of the equipment used to capture the data. Calibration ensures that the instruments provide accurate and reliable measurements, which is crucial for the success of the acquisition.
Examples:
The Acquisition (F2) of the 3D scan data was influenced by the calibration instrument (F108) to ensure the measurements were accurate.
The laser scanner (F2) used in the acquisition was influenced by calibration procedures (F108) to reduce systematic errors.
Label: was_influenced_by_calibration_instrument

Y131: used marker/calibration tool
URI: https://photogrammetry.altervista.org/items/show/390 
Subproperty of: P16 used specific object
Domain: F9 Acquisition Device
Range: F109 Marker and Calibration Tool
Scope Note:
	This property connects an Acquisition Device (F9) to a Marker or Calibration Tool (F109) used in the acquisition process. These tools are used to mark reference points or calibrate the device, ensuring accurate data capture during the acquisition phase. Markers and calibration tools are essential for improving the precision of the measurements, especially in complex environments.
Examples:
The Acquisition Device (F9) used markers and calibration tools (F109) to align the data capture accurately during the 3D scanning of the monument.
The laser scanner (F9) employed a calibration tool (F109) to improve the accuracy of the point cloud acquisition.
Label: used_marker_calibration_tool
—-------------------------------------------------------------------

Y132: had interactive application output
URI: https://photogrammetry.altervista.org/items/show/391 
Subproperty of: L11 had output
Domain: F92 Interactive Project Implementation
Range: F167 Interactive Application
Scope Note:
This property connects an Interactive Project Implementation (F92) to the Interactive Application (F167) that serves as the output of the project. It indicates that the interactive application is the result of the project, which may include a 3D model viewer, a virtual museum, or other interactive environments where users can explore or interact with the content. The output is the digital product delivered after the project implementation.
Examples:
The Interactive Project Implementation (F92) produced an Interactive Application (F167), which allowed users to explore the 3D model of an ancient city in a virtual environment.
After the Interactive Project Implementation (F92), the output was an interactive educational application (F167) that displayed historical data through augmented reality (AR).
Label: had_interactive_application_output

Y133: has interactive application description
URI: https://photogrammetry.altervista.org/items/show/392 
Subproperty of: P3 has note
Domain: F167 Interactive Application
Range: F125 Interactive Project Description
Scope Note:
	This property connects an Interactive Application (F167) to a description (F125) that outlines the purpose, functionality, and features of the application. The description provides context about how the interactive application operates, its goals, and the experiences it provides to users. This may include details on the user interface, interactivity features, and the content or models presented.
Examples:
The Interactive Application (F167) has an Interactive Project Description (F125) that explains the navigation features, including zooming, rotating, and exploring a virtual reconstruction of an ancient monument.
The description of the interactive application (F167) includes its role in a virtual museum, where users can interact with 3D models and gain insights into historical artifacts.
Label: has_interactive_application_description

Y134: has interactive project platform of developing
URI: https://photogrammetry.altervista.org/items/show/393 
Subproperty of: P16 used specific object
Domain: F92 Interactive Project Implementation
Range: F126 Interactive Project Platform
Scope Note:
	This property connects an Interactive Project Implementation (F92) to the specific platform used to develop and implement the interactive project (F126). The platform may refer to a software or development environment used to create the interactive experience, such as Unity, Unreal Engine, or other VR/AR development tools.
Examples:
The Interactive Project Implementation (F92) was developed using an Interactive Project Platform (F126) like Unity, which allowed for the creation of interactive 3D content.
The project was developed on the Unreal Engine platform (F126), and its implementation (F92) included virtual tours and educational content related to historical monuments.
Label: has_interactive_project_platform_of_developing

Y135: happened on multimedia device
URI: https://photogrammetry.altervista.org/items/show/394 
Subproperty of: L12 happened on modelling device
Domain: F167 Interactive Application
Range: F128 Interactive Project Running Device
Scope Note:
	This property links an Interactive Application (F167) to the Multimedia Device (F128) on which the application is run or executed. The multimedia device could refer to a computer, tablet, smartphone, VR headset, or any other hardware that runs the interactive application. The property highlights the role of the device in presenting or running the interactive experience.
Examples:
The Interactive Application (F167) happened on a multimedia device (F128) such as an Oculus VR headset, providing an immersive virtual tour experience.
The educational AR application (F167) was run on multimedia devices (F128), like smartphones and tablets, enabling users to interact with historical data via augmented reality.
Label: happened_on_multimedia_device



—------------------------------------------------------------

F170 Acquisition Environment Type
URI: https://photogrammetry.altervista.org/items/show/407 
Subclass of: E55 Type
Scope Note:
	This class represents the type of environment in which the acquisition took place. It categorizes the setting—such as indoor, outdoor, underwater, cave, urban area, or desert—where the surveying or photogrammetric process was conducted. Defining the acquisition environment type helps in contextualizing the conditions under which data was captured, influencing factors like lighting, accessibility, stability of the setup, and potential obstructions.
Examples:
The acquisition was performed in a controlled indoor environment with stable lighting conditions.
The survey took place in an open-air archaeological site under natural lighting and uneven ground conditions.
Label: AcquisitionEnvironmentType
—-----------------------------------------------------------------------

Y136: has EIS project identifier


URI: https://photogrammetry.altervista.org/items/show/410 
Subproperty of: P1 is identified by
Domain: F89 Project Analysis
Range: F137 Environmental Impact Studies Project Title/DOI
Scope Note:
	This property links a Project Analysis (F89) to its Environmental Impact Studies (EIS) project identifier (F137), typically a title or DOI. It ensures that the EIS project can be referenced and retrieved easily.
Examples:
A Project Analysis (F89) has an EIS project identifier (F137) "EIS_DOI_10.1234/environmental.impact" allowing for quick lookup of related environmental studies.

Label: has_EIS_project_identifier

Y137: has surface detail resolution


URI: https://photogrammetry.altervista.org/items/show/411 
Subproperty of: P43 has dimension
Domain: F88 3D Model for Research
Range: F146 Surface Detail Resolution
Scope Note:
	This property associates a 3D Model for Research (F88) with its surface detail resolution (F146), expressed as a dimension or measurement. It ensures that the level of fine detail captured by the model is clearly recorded.
Examples:


A 3D Model for Research (F88) has a surface detail resolution (F146) of 0.02 mm, indicating a highly detailed mesh suitable for microanalysis.

Label: has_surface_detail_resolution

Y138: gives material tolerance requirements


URI:https://photogrammetry.altervista.org/items/show/409 
Subproperty of: P140 assigned attribute to
Domain: F147 Material Tolerance Requirements
Range: F78 Material for 3D Printing
Scope Note:
	This property connects Material Tolerance Requirements (F147) with a Material for 3D Printing (F78), specifying the tolerance levels needed in the printing material. This ensures that the chosen printing material meets the exacting precision standards required by the model.
Examples:
Material Tolerance Requirements (F147) gives material tolerance requirements to a specific Material for 3D Printing (F78) that needs a tolerance of ±0.05 mm to achieve the desired dimensional accuracy.

Label: gives_material_tolerance_requirements

Y139: gives scaling factor ratio


URI: https://photogrammetry.altervista.org/items/show/408 
Subproperty of: P140 assigned attribute to
Domain: F148 Scaling Factor
Range: F59 Digital Scale
Scope Note:
	This property links the Scaling Factor (F148) to a Digital Scale (F59), indicating the ratio at which the model is represented (e.g., 1:1, 1:10). Recording this scaling factor is crucial for analyses, comparisons, or producing accurate replicas.
Examples:
A Scaling Factor (F148) gives a scaling factor ratio (F59) of 1:5, indicating the model is reduced to one-fifth of the artifact’s original size.

Label: gives_scaling_factor_ratio

Y140: uses specific production method compatibility
URI: https://photogrammetry.altervista.org/items/show/412 
Subproperty of: P33 used specific technique
Domain: F77 Printing Digital Twin
Range: F149 Production Method Compatibility
Scope Note:
	This property indicates that a Printing Digital Twin (F77) utilizes a specific Production Method Compatibility (F149), ensuring that the chosen printing or fabrication technique (e.g., SLA, FDM, resin casting) aligns with the requirements of the model.
Examples:
A Printing Digital Twin (F77) uses specific production method compatibility (F149) that supports SLS (Selective Laser Sintering), confirming that the model can be successfully printed with this technology.

Label: uses_specific_production_method_compatibility
 —---------------------------------------------------------------------
Y141: has baseline dataset date

URI: https://photogrammetry.altervista.org/items/show/413 
Subproperty of: P4 has time-span
Domain: F88 3D Model for Research
Range: F150 Baseline Dataset Date
Scope Note:
	This property associates a 3D Model for Research (F88) with a Baseline Dataset Date (F150), indicating the reference temporal point from which changes and evolutions of the model will be monitored over time. By specifying the baseline date, users can track modifications, updates, or degradations in the 3D model over its lifecycle.
Examples:


A 3D Model for Research (F88) has a baseline dataset date (F150) recorded as “2021-06-15,” serving as the reference date for all subsequent analyses.
Label: has_baseline_dataset_date

Y142: is referred to a specific S.U.

URI: https://photogrammetry.altervista.org/items/show/414 
Subproperty of: P7 took place at
Domain: F89 Project Analysis
Range: F138 S.U. Referenced Place of Excavation
Scope Note:
	This property links a Project Analysis (F89) focused on archaeometric or other in-depth studies to the Stratigraphic Unit (S.U.) referenced excavation place (F138) associated with the 3D model’s original find context. It ensures a clear connection between the project’s analysis and the precise excavation context, aiding in archaeological interpretation and contextualization.
Examples:


A Project Analysis (F89) focusing on pottery composition is referred to a specific S.U. (F138), indicating the ceramic fragments originated from a distinct stratigraphic level.
Label: is_referred_to_a_specific_SU

Y143: has main face

URI: https://photogrammetry.altervista.org/items/show/415 
Subproperty of: P140i was attributed by
Domain: F100 Digital Twin
Range: F157 Identified Main Face
Scope Note:
	This property indicates that a Digital Twin (F100) has an identified main face (F157), a crucial reference surface chosen for alignment, registration, or interpretive purposes. Assigning a main face provides a consistent reference for analyzing or comparing complex 3D models.
Examples:


A Digital Twin (F100) of a ceramic vessel has a main face (F157) designated as the flat base, used as a reference plane for all subsequent alignment tasks.
Label: has_main_face

Y144: has model multiple composition

URI: https://photogrammetry.altervista.org/items/show/416 
Subproperty of: P140i was attributed by
Domain: F100 Digital Twin
Range: F156 Model Composition from Multiple Parts
Scope Note:
	This property specifies that a Digital Twin (F100) is composed of multiple parts (F156) integrated into one coherent model. It records the relationship between a unified 3D representation and its segmented origins, highlighting the complexity of the reconstruction process.
Examples:


A Digital Twin (F100) of a large statue has model multiple composition (F156), indicating it was assembled from several individually scanned segments.
Label: has_model_multiple_composition

Y145: has carried out comparison activity on 3D model

URI: https://photogrammetry.altervista.org/items/show/417 
Subproperty of: P140 assigned attribute to
Domain: F142 Comparison Activity of Different 3D Models
Range: F100 Digital Twin
Scope Note:
	This property denotes that a Comparison Activity (F142) has been performed on a specific Digital Twin (F100). It captures the action of measuring discrepancies, deviations, or similarities between multiple 3D models.
Examples:


A Comparison Activity (F142) has carried out comparison activity on a 3D model (F100), identifying differences between two digital twins of the same artifact taken months apart.
Label: has_carried_out_comparison_activity_on_3D_model

Y146: used comparison software

URI: https://photogrammetry.altervista.org/items/show/418 
Subproperty of: P16 used specific object
Domain: F142 Comparison Activity of Different 3D Models
Range: F144 Software Used for the Comparison of Two 3D Models
Scope Note:
	This property connects a Comparison Activity (F142) to the specific comparison software (F144) employed in the analysis. It ensures transparency in the tools and methods used to derive insights from multiple 3D models.
Examples:
A Comparison Activity (F142) used comparison software (F144) like CloudCompare to detect surface deviations between two digital twins.
Label: used_comparison_software

Y147: used comparison method
URI: https://photogrammetry.altervista.org/items/show/419 
Subproperty of: P33 used specific technique
Domain: F142 Comparison Activity of Different 3D Models
Range: F145 Methodology Adopted for the Comparison
Scope Note:
	This property indicates that a Comparison Activity (F142) was guided by a specific comparison methodology (F145). It records the analytical approach or algorithmic procedure chosen for evaluating differences or similarities between 3D models.
Examples:
A Comparison Activity (F142) used comparison method (F145) involving point-to-point distance calculation to quantify differences between two aligned meshes.
Label: used_comparison_method

Y148: S.U. has coordinates

URI: https://photogrammetry.altervista.org/items/show/420 
Subproperty of: P168 place is defined by
Domain: F138 S.U. Referenced Place of Excavation
Range: F139 S.U. Coordinates
Scope Note:
	This property links a Stratigraphic Unit’s referenced place (F138) with its spatial coordinates (F139), defining the exact location of the S.U. within the excavation site. Such geospatial referencing is vital for archaeological contextualization and subsequent analysis.
Examples:


An S.U. Referenced Place of Excavation (F138) has coordinates (F139) recorded as UTM 33T E500000 N4640000.
Label: SU_has_coordinates

Y149: was S.U. characterized by material

URI: https://photogrammetry.altervista.org/items/show/421 
No subproperty
Domain: F138 S.U. Referenced Place of Excavation
Range: F140 S.U. Material
Scope Note:
	This property notes that a Stratigraphic Unit (F138) was characterized by a particular material (F140), such as sediment type, soil composition, or artifact concentration. Understanding these material characteristics aids in interpreting the archaeological context and depositional history.
Examples:


An S.U. Referenced Place of Excavation (F138) was characterized by material (F140) predominantly composed of clay and small ceramic sherds.
Label: was_SU_characterized_by_material

Y150: has orientation of 3D model

URI: https://photogrammetry.altervista.org/items/show/422 
Subproperty of: P140i was attributed by
Domain: F100 Digital Twin, F81 3D Model for G.I.S, F88 3D Model for Research
Range: F155 Orientation of the 3D Model
Scope Note:
	This property associates a Digital Twin (F100), a 3D Model for GIS (F81), or a 3D Model for Research (F88) with its orientation (F155), reflecting how the model is placed or aligned within a coordinate system. Recording orientation ensures consistency across analyses and visualizations.
Examples:


A Digital Twin (F100) has orientation of 3D model (F155) defined by a rotation of 45° around the Z-axis.
Label: has_orientation_of_3D_model

Y151: has 3d model spatial metadata
URI: https://photogrammetry.altervista.org/items/show/423 
Subproperty of: P140i was attributed by
Domain: F100 Digital Twin, F81 3D Model for G.I.S, F88 3D Model for Research
Range: F153 3D Model Spatial Metadata
Scope Note:
	This property links a 3D model (in various contexts) to its spatial metadata (F153), covering aspects like georeferencing, orientation, and composition. By recording this metadata, users can better interpret the model’s spatial parameters and integrate it with other spatial datasets.
Examples:


A 3D Model for Research (F88) has 3D model spatial metadata (F153) detailing its georeference system and assembled composition.
Label: has_3D_model_spatial_metadata

Y152: has 3d model georeferencing

URI: https://photogrammetry.altervista.org/items/show/424 
Subproperty of: P140i was attributed by
Domain: F100 Digital Twin, F81 3D Model for G.I.S, F88 3D Model for Research
Range: F154 Georeferencing of the 3D Model
Scope Note:
	This property specifies that a given 3D model is georeferenced (F154), linking its coordinates to a known spatial reference system. Georeferencing supports integration with maps, GIS layers, and other spatial analyses.
Examples:
A 3D Model for GIS (F81) has 3D model georeferencing (F154) aligned to the WGS84 coordinate system.
Label: has_3D_model_georeferencing

Y153: has 3d model density and uniformity
URI: [insert URI here]
Subproperty of: P43 has dimension
Domain: F88 3D Model for Research
Range: F158 Mesh Density and Uniformity
Scope Note:
	This property associates a research-oriented 3D model (F88) with its mesh density and uniformity (F158), quantifying how consistently its geometry is distributed. Such information is vital for simulations and structural analyses requiring homogeneous mesh quality.
Examples:


A 3D Model for Research (F88) has 3d model density and uniformity (F158) indicating an average face size of 0.1 mm and uniform distribution.
Label: has_3D_model_density_and_uniformity

Y154: has material properties assignment

URI: https://photogrammetry.altervista.org/items/show/425 
Subproperty of: O16i value was observed by
Domain: F88 3D Model for Research
Range: F159 Material Properties Assignment
Scope Note:
This property identifies that the material properties (F159) have been assigned or observed for a 3D Model for Research (F88). Such properties might include density, elasticity, or compressive strength, enabling more accurate simulations and analyses.
Examples:
A 3D Model for Research (F88) has material properties assignment (F159) where steel’s density and Young’s modulus are recorded.
Label: has_material_properties_assignment

Y155: has boundary and constraints

URI: https://photogrammetry.altervista.org/items/show/426 
No subproperty
Domain: F88 3D Model for Research
Range: F160 Boundary Conditions and Constraints
Scope Note:
	This property links a 3D Model for Research (F88) to the boundary conditions and constraints (F160) applied, essential for structural or mechanical simulations. Recording these ensures replicability and correct interpretation of simulation results.
Examples:


A 3D Model for Research (F88) has boundary and constraints (F160) defining fixed supports at its base and a uniform load along its top edge.
Label: has_boundary_and_constraints

Y156: has load parameters

URI: https://photogrammetry.altervista.org/items/show/427 
Subproperty of: P3 has note
Domain: F88 3D Model for Research
Range: F162 Structural Load Parameters
Scope Note:
	This property attaches load parameter data (F162) to a research-oriented 3D model (F88). It clarifies what types of loads (e.g., static, dynamic) and units (e.g., N, kPa) are involved, enabling precise simulations or assessments of structural behavior.
Examples:


A 3D Model for Research (F88) has load parameters (F162) indicating a static vertical load of 1000 N applied to its top surface.
Label: has_load_parameters






























Thesauruses and Vocabularies

For some specific classes, a thesaurus of terms is suggested to be adopted to express some concepts in a standard way. The thesauri are partly taken from the FOPPA Manual and the studies related to it, partly they were produced specifically for PODS.

Thesaurus for F101 Survey Phase 
The following terms do not define an absolute chronological value (for which reference is made to the F43 Date of Acquisition class) but a relative temporal value, i.e. how the survey is placed in relation to the project times and the role it has in relation to potential previous surveys that may have concerned the surveyed object.

ALFA: 
First Survey Coincident with the discovery or first survey project
https://photogrammetry.altervista.org/items/show/337 

rdfs:label: ALFA  
skos:definition: First survey coincident with the discovery or first survey project.  
skos:altLabel: Initial Survey, Primary Survey Phase  
dcterms:source: PODS Declaration  
skos:scopeNote: Use this term to describe the very first survey conducted on an object, coinciding with its discovery or its inclusion in an initial survey project.  
owl:versionInfo: 1.0  
dcterms:description: Defines the first phase of a survey project, typically coinciding with the initial examination or discovery of the object or site.  
rdfs:seeAlso: https://www.wikidata.org/wiki/Q94701573 
dcterms:modified: 2024-11-29  
dcterms:creator: Vittorio Lauro  

BETA: 
First Survey on a classified object for more than 2 years
https://photogrammetry.altervista.org/items/show/371 
rdfs:label: BETA  
skos:definition: First survey on a classified object conducted after more than 2 years.  
skos:altLabel: Delayed Primary Survey, Post-Classification Survey  
dcterms:source: PODS Declaration  
skos:scopeNote: Use this term to define the initial survey on an object that has already been classified but is being revisited after a significant temporal gap of more than 2 years.  
owl:versionInfo: 1.0  
dcterms:description: Represents a survey phase where an object is examined for the first time following its classification, usually after a period exceeding two years.  
rdfs:seeAlso: https://www.wikidata.org/wiki/Q94701573   
dcterms:modified: 2024-12-6  
dcterms:creator: Vittorio Lauro 

GAMMA: 
Second survey on an already surveyed object
https://photogrammetry.altervista.org/items/show/372 

rdfs:label: GAMMA  
skos:definition: Second survey conducted on an object already surveyed.  
skos:altLabel: Follow-Up Survey, Secondary Survey Phase  
dcterms:source: PODS Declaration  
skos:scopeNote: Use this term to describe a subsequent survey phase on an object that has already been the subject of a prior survey, allowing for comparative analysis or updated data collection.  
owl:versionInfo: 1.0  
dcterms:description: Defines the phase of a survey project in which an object or site is reexamined, typically for validation, updates, or refinement of data.  
rdfs:seeAlso: https://www.wikidata.org/wiki/Q94701573   
dcterms:modified: 2024-12-6  
dcterms:creator: Vittorio Lauro  

DELTA: 
Third survey an already surveyed object
https://photogrammetry.altervista.org/items/show/373 
rdfs:label: DELTA  
skos:definition: Third survey conducted on an already surveyed object.  
skos:altLabel: Tertiary Survey, Third-Phase Survey  
dcterms:source: PODS Declaration  
skos:scopeNote: Use this term to describe a third survey phase conducted on an object that has already been surveyed at least twice, often for further validation or refinement of previous data.  
owl:versionInfo: 1.0  
dcterms:description: Represents the third phase of a survey conducted on an object previously examined, usually as part of ongoing research or to capture evolving details.  
rdfs:seeAlso: https://www.wikidata.org/wiki/Q94701573   
dcterms:modified: 2024-11-25  
dcterms:creator: Vittorio Lauro

EPSILON: 
over the third survey of an already surveyed object
https://photogrammetry.altervista.org/items/show/374 
rdfs:label: EPSILON  
skos:definition: Fourth or subsequent survey conducted on an already surveyed object.  
skos:altLabel: Quaternary Survey, Extended Survey  
dcterms:source: PODS Declaration  
skos:scopeNote: Use this term to describe a survey conducted after the third or more surveys on an object, typically indicating deeper investigation or updates to previous survey data.  
owl:versionInfo: 1.0  
dcterms:description: Defines the phase of a survey where an object is subject to an additional round of documentation or refinement after several prior surveys.  
rdfs:seeAlso: https://www.wikidata.org/wiki/Q94701573   
dcterms:modified: 2024-12-6  
dcterms:creator: Vittorio Lauro  

ZETA: 
Survey of a 3d print of surveyed object
https://photogrammetry.altervista.org/items/show/375 
rdfs:label: ZETA  
skos:definition: Survey of a 3D print of a surveyed object.  
skos:altLabel: 3D Print Survey, Printed Model Survey  
dcterms:source: PODS Declaration  
skos:scopeNote: Use this term to describe a survey phase where a 3D print of a previously surveyed object is surveyed, often for comparison, quality assurance, or analysis.  
owl:versionInfo: 1.0  
dcterms:description: Defines the survey phase where a physical 3D printed replica of an object undergoes documentation and analysis, mirroring the original object’s survey data.  
rdfs:seeAlso: https://www.wikidata.org/wiki/Q94701573   + https://www.wikidata.org/wiki/Q229367 
dcterms:modified: 2024-12-6 
dcterms:creator: Vittorio Lauro  

ETA: 
Virtual survey of a 3d survey in virtual context
https://photogrammetry.altervista.org/items/show/376 
rdfs:label: ETA  
skos:definition: Virtual survey of a 3D survey in a virtual context.  
skos:altLabel: Virtual 3D Survey, Digital Surveying  
dcterms:source: PODS Declaration  
skos:scopeNote: Use this term to refer to a survey performed on a 3D model or a scanned object in a virtual environment, often for visualization, analysis, or manipulation within digital or augmented spaces.  
owl:versionInfo: 1.0  
dcterms:description: Represents a virtual survey phase, where a 3D scanned object or model is analyzed within a digital or virtual space, facilitating advanced study, interaction, and visualization.  
rdfs:seeAlso: https://www.wikidata.org/wiki/Q94701573   
dcterms:modified: 2024-12-6  
dcterms:creator: Vittorio Lauro 



Thesaurus for F12 Acquisition Trajectory
Path Used for the survey:
fs: freehand spiral
https://photogrammetry.altervista.org/items/show/395 
The Spiral Acquisition method in the F.O.P.P.A. protocol systematically captures detailed information by focusing on an object's center, starting with perpendicular shots, then 45° and 75° inclinations. It effectively documents finds from multiple perspectives, emphasizing intricate details and adapting to cavities or corridor-like structures. Further information in the FOPPA Manual

rdfs:label: fs (Freehand Spiral)  
skos:definition: The Spiral Acquisition method systematically captures detailed information by focusing on an object's center, beginning with perpendicular shots, then 45° and 75° inclinations.  
skos:altLabel: Spiral Acquisition Method  
dcterms:source: FOPPA Manual  
skos:scopeNote: Used for capturing objects from multiple perspectives, especially for documenting intricate details, particularly for complex or cavity-like structures.  
owl:versionInfo: 1.0  
dcterms:description: A method that allows detailed documentation of objects with complex structures, facilitating precise acquisition of 3D models.  
rdfs:seeAlso: https://www.wikidata.org/wiki/Q94701573 P2079  https://www.wikidata.org/wiki/Q193139 P737 https://www.wikidata.org/wiki/Q6482775 P1449  https://www.wikidata.org/wiki/Q17278   
dcterms:modified: 2024-12-10  
dcterms:creator: Vittorio Lauro  

lf: linear freehand
https://photogrammetry.altervista.org/items/show/396 
The Straight Line Acquisition method in the F.O.P.P.A. protocol surveys large buildings by moving the camera parallel to the structure while keeping it perpendicular. It ensures comprehensive coverage and captures intricate details. Maintaining at least 70% overlap between photos is crucial for accurate 3D model reconstruction and minimizing missed details. Further information in the FOPPA Manual

rdfs:label: lf (Linear Freehand)  
skos:definition: The Straight Line Acquisition method surveys large buildings by moving the camera parallel to the structure while maintaining perpendicularity.  
skos:altLabel: Linear Freehand Method  
dcterms:source: FOPPA Manual  
skos:scopeNote: Ensures comprehensive coverage of large structures and emphasizes intricate details, requiring at least 70% overlap for accurate 3D reconstruction.  
owl:versionInfo: 1.0  
dcterms:description: Used to survey large buildings or extensive structures where maintaining proper overlap between images is essential for precise model creation.  
rdfs:seeAlso:  https://www.wikidata.org/wiki/Q94701573 P2079  https://www.wikidata.org/wiki/Q193139 P737 https://www.wikidata.org/wiki/Q6482775 P1449 https://www.wikidata.org/wiki/Q37105 
dcterms:modified: 2024-12-10  
dcterms:creator: Vittorio Lauro  

ad: aerial wireless
https://photogrammetry.altervista.org/items/show/397 
The Aerial Acquisition technique in the F.O.P.P.A. protocol involves moving parallel to the ground with a downward-tilted camera, ideal for drones. It effectively documents archaeological trenches and extensive territories, providing comprehensive, elevated images for detailed data collection and insights into spatial layout and features.  Further information in the FOPPA Manual

rdfs:label: ad (Aerial Wireless)  
skos:definition: The Aerial Acquisition technique involves moving parallel to the ground with a downward-tilted camera, ideal for drone-based surveys.  
skos:altLabel: Aerial Acquisition, Drone Survey  
dcterms:source: PODS Thesaurus   
skos:scopeNote: Ideal for surveying archaeological trenches, large areas, or territories, providing elevated and comprehensive views for detailed spatial data collection.  
owl:versionInfo: 2.0  
dcterms:description: A method for large-scale surveys where aerial perspectives provide essential insights into spatial features and landscape data, often used with drone technologies.  
rdfs:seeAlso:  https://www.wikidata.org/wiki/Q94701573 P2079  https://www.wikidata.org/wiki/Q4688034 P737 https://www.wikidata.org/wiki/Q484000   
dcterms:modified: 2024-12-10  
dcterms:creator: Vittorio Lauro  

vl: vertical or with drone or with rod
https://photogrammetry.altervista.org/items/show/398 
Vertical capture in the F.O.P.P.A. protocol involves systematic image acquisition along a vertical plane, ideal for tall structures. Drones or cameras on poles are recommended for flexibility and efficiency, ensuring comprehensive documentation of elevations like architectural elements and monuments. Further information in the FOPPA Manual

rdfs:label: vl (Vertical or with Drone or with Rod)  
skos:definition: Vertical capture involves systematic image acquisition along a vertical plane, suitable for tall structures. Drones or cameras on rods are recommended for flexibility and efficiency.  
skos:altLabel: Vertical Capture, Drone or Rod Capture  
dcterms:source: FOPPA Manual  
skos:scopeNote: This method is primarily used for capturing architectural elevations and monuments, ensuring thorough documentation of vertical surfaces.  
owl:versionInfo: 1.0  
dcterms:description: Vertical survey ideal for tall objects, including architectural elements, using drones or camera-mounted poles for effective documentation.  
rdfs:seeAlso:  https://www.wikidata.org/wiki/Q94701573 P2079  https://www.wikidata.org/wiki/Q193139 P737 https://www.wikidata.org/wiki/Q6482775 P1449  https://www.wikidata.org/wiki/Q484000   
dcterms:modified: 2024-12-10  
dcterms:creator: Vittorio Lauro  

sb: spiral with rotating base
https://photogrammetry.altervista.org/items/show/399 
The rotating base survey in the F.O.P.P.A. protocol involves rotating the object on a neutral-colored base with four camera positions (0°, 15°, 45°, 75°). The base rotates 5-15° between photos, ensuring detailed capture. Reflective objects require an absorbent background like velvet. Further information in the FOPPA Manual

rdfs:label: sb (Spiral with Rotating Base)  
skos:definition: A rotating base survey involves rotating the object on a neutral-colored base with four camera positions (0°, 15°, 45°, 75°), capturing images at each rotation angle.  
skos:altLabel: Rotating Base Survey, Spiral Base Method  
dcterms:source: PODS Thesaurus   
skos:scopeNote: Used for capturing reflective objects with an absorbent background, ensuring a detailed, comprehensive documentation process.  
owl:versionInfo: 2.0  
dcterms:description: A survey method using a rotating base for precise capturing of objects with a 5-15° increment, ideal for reflective surfaces.  
rdfs:seeAlso: https://www.wikidata.org/wiki/Q94701573 P2079 https://www.wikidata.org/wiki/Q111973380   
dcterms:modified: 2024-12-10  
dcterms:creator: Vittorio Lauro  

 el: easel linear
https://photogrammetry.altervista.org/items/show/400 
Acquisition with a camera fixed on a tripod involves moving the camera laterally at equidistant points, perpendicular to the object. It's useful for analyzing walls with small, colorimetrically distinct features. Each photo must overlap at least 70% with the preceding one, requiring numerous acquisitions. Further information in the FOPPA Manual

rdfs:label: el (Easel Linear)  
skos:definition: Acquisition with a camera fixed on a tripod involves lateral camera movement at equidistant points, perpendicular to the object, ensuring 70% overlap.  
skos:altLabel: Easel Camera Survey, Tripod Linear Survey  
dcterms:source: FOPPA Manual  
skos:scopeNote: Ideal for small, color-distinct features, typically used for walls with intricate details and small object analysis.  
owl:versionInfo: 1.0  
dcterms:description: Used for detailed documentation of small objects, ensuring precise lateral movements and overlap between photos.  
rdfs:seeAlso:  https://www.wikidata.org/wiki/Q94701573 P2079  https://www.wikidata.org/wiki/Q193139 P737 https://www.wikidata.org/wiki/Q6482775 P1449 https://www.wikidata.org/wiki/Q37105 + https://www.wikidata.org/wiki/Q1444534   
dcterms:modified: 2024-12-10  
dcterms:creator: Vittorio Lauro  

 sm: structured mixed
https://photogrammetry.altervista.org/items/show/401 
Structured mixed acquisition combines linear, spiral, and vertical surveys, adhering to the parameters of each method. While generally avoided for large structures, it's effective for irregular small objects and body parts. Specific guidelines for human body part surveys are detailed in Appendix #1 of the FOPPA Manual.

rdfs:label: sm (Structured Mixed)  
skos:definition: Structured mixed acquisition combines linear, spiral, and vertical surveys, adapting each method to its specific parameters.  
skos:altLabel: Mixed Acquisition, Multi-Method Survey  
dcterms:source: FOPPA Manual  
skos:scopeNote: Effective for irregular small objects and body parts, though generally avoided for large structures. Specific guidelines for human body parts are in Appendix #1 of the FOPPA Manual.  
owl:versionInfo: 1.0  
dcterms:description: Combines different survey techniques for capturing complex or irregularly shaped objects, particularly human body parts.  
rdfs:seeAlso:  https://www.wikidata.org/wiki/Q94701573   
dcterms:modified: 2024-12-10  
dcterms:creator: Vittorio Lauro  

mu: mixed unstructured
https://photogrammetry.altervista.org/items/show/402 
Unstructured mixed acquisition is used for irregular environments where standard modules don't apply. It requires photos to share at least 80% of representation, maintaining camera orientation. This method is necessary for areas like deep tunnels and involves taking numerous photographs to ensure detailed coverage. Further information in the FOPPA Manual

rdfs:label: mu (Mixed Unstructured)  
skos:definition: Unstructured mixed acquisition is used in irregular environments where standard modules do not apply, requiring at least 80% photo overlap with consistent camera orientation.  
skos:altLabel: Unstructured Mixed Acquisition, Irregular Environment Survey  
dcterms:source: FOPPA Manual  
skos:scopeNote: Used in environments like deep tunnels where conventional survey methods do not fit, ensuring detailed coverage by taking numerous photographs.  
owl:versionInfo: 1.0  
dcterms:description: Ideal for complex, irregular environments, ensuring comprehensive capture of areas that traditional methods can't address.  
rdfs:seeAlso:  https://www.wikidata.org/wiki/Q94701573  
dcterms:modified: 2024-12-10  
dcterms:creator: Vittorio Lauro  
rm: rotating base microscope
https://photogrammetry.altervista.org/items/show/403 
Rotating base acquisitions with a microscope camera are tailored for objects smaller than 2cm. Specific measures address challenges like orthographic lens effects and precise acquisition point management. Appendix #2 of the FOPPA Protocol extensively covers these methods for acquiring tiny objects. 

rdfs:label: rm (Rotating Base Microscope)  
skos:definition: Rotating base acquisitions with a microscope camera are used for objects smaller than 2 cm, addressing challenges like orthographic lens effects and acquisition point management.  
skos:altLabel: Rotating Base Microscope Acquisition, Microscope Camera Survey  
dcterms:source: FOPPA Manual  
skos:scopeNote: Applied to small objects under 2 cm, this method ensures precise and detailed acquisition, accounting for small-scale intricacies.  
owl:versionInfo: 1.0  
dcterms:description: Specialized for tiny objects, it utilizes a microscope with a rotating base to capture fine details under challenging conditions.  
rdfs:seeAlso: https://www.wikidata.org/wiki/Q94701573 P2079 https://www.wikidata.org/wiki/Q111973380  + https://www.wikidata.org/wiki/Q196538   
dcterms:modified: 2024-12-10  
dcterms:creator: Vittorio Lauro  

rb: rotating base fixed instrument
https://photogrammetry.altervista.org/items/show/404 
This category includes all those acquisitions in which the acquisition instrument has a fixed position and the specimen is rotated to be exposed in all its parts to the sensor. This category includes, for example, hybrid instruments of the photogrammetric and laser scanner category (such as the ATOS III) or the box laser scanner.

rdfs:label: rb (Rotating Base Fixed Instrument)  
skos:definition: This category involves acquisitions where the instrument is fixed and the specimen is rotated to expose all parts to the sensor, used in hybrid photogrammetric and laser scanner instruments.  
skos:altLabel: Rotating Base Fixed Instrument Survey, Fixed Instrument Acquisition  
dcterms:source: PODS Thesaurus   
skos:scopeNote: Commonly applied in systems like the ATOS III, which integrates photogrammetry and laser scanning for comprehensive 3D scanning.  
owl:versionInfo: 2.0  
dcterms:description: Used in photogrammetric and laser scanner hybrid instruments to capture detailed data through rotating specimens.  
rdfs:seeAlso: https://www.wikidata.org/wiki/Q94701573 P2079 https://www.wikidata.org/wiki/Q111973380  + https://www.wikidata.org/wiki/Q196538 + https://www.wikidata.org/wiki/Q1444534  
dcterms:modified: 2024-12-10  
dcterms:creator: Vittorio Lauro  



Thesaurus for F19 Scale Type F18 Dominant Geometry Type
Scale of the Surveyed Object:
A: Small object (equal to or smaller than 1 cm)
https://photogrammetry.altervista.org/items/show/405 
Small objects mean those archaeological finds of any material that have a diameter equal to or less than 1 cm. Complete objects originally of small size fall into this category, as do fragments of small objects.

rdfs:label: A (Small Object - Equal to or Smaller than 1 cm)  
skos:definition: Small objects mean those archaeological finds of any material that have a diameter equal to or less than 1 cm, including complete objects or fragments of small items.  
skos:altLabel: Small Object, Tiny Find  
dcterms:source: PODS Thesaurus  
skos:scopeNote: Includes both complete small objects and fragments of such items, often requiring detailed and precise documentation.  
owl:versionInfo: 1.0  
dcterms:description: Small archaeological objects that are 1 cm or smaller, significant in archaeological study for their detailed analysis.  
rdfs:seeAlso: 
:SmallObject a owl:Class ;
    rdfs:label "Small Object"@en ;
    rdfs:comment "Objects with a volume equal to or smaller than a cube with 1cm edge length."@en ;
    skos:definition "Any object whose volume is ≤ 1 cm³, corresponding to a cube with edges of 1 cm."@en ;
    :hasMaximumDimension [
        a owl:Restriction ;
        owl:onProperty :edgeLength ;
        owl:allValuesFrom [
            a rdfs:Datatype ;
            owl:onDatatype xsd:decimal ;
            owl:withRestrictions (
                [ xsd:maxInclusive "1.0"^^xsd:decimal ]
            )
        ] ;
    ] .

 
dcterms:modified: 2024-12-5  
dcterms:creator: Vittorio Lauro 


B: Medium Object (1cm to 30cm)
https://photogrammetry.altervista.org/items/show/406 
Objects whose diameter is between 1 cm and 30 cm, even partial parts of a larger overall object. In the case of extremely irregular objects, consider the maximum extension diameter.

rdfs:label: B (Medium Object - 1 cm to 30 cm)  
skos:definition: Objects whose diameter ranges between 1 cm and 30 cm, including partial parts of larger objects, or in the case of irregular objects, the maximum extension diameter.  
skos:altLabel: Medium Object, Medium-Sized Find  
dcterms:source: PODS Thesaurus  
skos:scopeNote: Covers objects of medium size, often partial pieces or irregular objects where the maximum measurement is taken.  
owl:versionInfo: 1.0  
dcterms:description: Includes objects that fit within the 1 cm to 30 cm range, requiring medium-scale surveys and detailed documentation.  
rdfs:seeAlso: 
:MediumObject a owl:Class ;
    rdfs:label "Medium Object"@en ;
    rdfs:comment "Objects with an edge length between 1 cm and 30 cm."@en ;
    skos:definition "Any object whose edge length is ≥ 1 cm and ≤ 30 cm."@en ;
    :hasEdgeLength [
        a owl:Restriction ;
        owl:onProperty :edgeLength ;
        owl:allValuesFrom [
            a rdfs:Datatype ;
            owl:onDatatype xsd:decimal ;
            owl:withRestrictions (
                [ xsd:minInclusive "1.0"^^xsd:decimal ]
                [ xsd:maxInclusive "30.0"^^xsd:decimal ]
            )
        ] ;
    ] .



 
dcterms:modified: 2024-12-5  
dcterms:creator: Vittorio Lauro  


C: Large Object (from 30 cm upwards)
Objects whose diameter is equal to or greater than 30 cm. The objects can be removable or immovable, of any material but they must have the characteristic of not being able to access the inside, therefore they cannot be visited. The Statue of Liberty does not fall into this category.

rdfs:label: C (Large Object - 30 cm and Above)  
skos:definition: Objects whose diameter is equal to or greater than 30 cm, including removable and immovable objects, which cannot be accessed internally or visited.  
skos:altLabel: Large Object, Large-Scale Find  
skos:broader: Scale Type, Dominant Geometry Type  
skos:related: Archaeological Object Size  
dcterms:identifier: C  
dcterms:source: PODS Thesaurus  
dcterms:language: en  
skos:scopeNote: Encompasses large archaeological objects that cannot be accessed internally, such as large statues or immovable objects.  
owl:versionInfo: 1.0  
dcterms:status: Approved  
dcterms:description: Objects with a diameter of 30 cm or more, requiring specialized equipment and techniques for documentation and analysis.  
rdfs:seeAlso: 
:LargeObject a owl:Class ;
    rdfs:label "Large Object"@en ;
    rdfs:comment "Objects with an edge length equal to or greater than 30 cm."@en ;
    skos:definition "Any object whose edge length is ≥ 30 cm."@en ;
    :hasEdgeLength [
        a owl:Restriction ;
        owl:onProperty :edgeLength ;
        owl:allValuesFrom [
            a rdfs:Datatype ;
            owl:onDatatype xsd:decimal ;
            owl:withRestrictions (
                [ xsd:minInclusive "30.0"^^xsd:decimal ]
            )
        ] ;
    ] .



 
skos:inScheme: F19 Scale Type Thesaurus  
dcterms:created: 2024-11-25  
dcterms:modified: 2024-12-5  
dcterms:creator: Vittorio Lauro  


D: Open architectural structure
https://photogrammetry.altervista.org/items/show/428 
Architectural structures that can be visited or potentially visited, understood in their overall external structure and not in their internal volumes. Courtyards and parade grounds fall into this category as they are external volumes.

rdfs:label: D (Open Architectural Structure)  
skos:definition: Architectural structures that can be visited or potentially visited, understood in their overall external structure and not in their internal volumes. Examples include courtyards and parade grounds, which are external volumes.  
skos:altLabel: Open Structure, External Architectural Structure  
dcterms:source: FOPPA Manual  
dcterms:language: en  
skos:scopeNote: Refers to external architectural volumes that are accessible or potentially accessible, excluding internal spaces.  
owl:versionInfo: 1.0  
dcterms:status: Approved  
dcterms:description: Describes architectural structures that are open for visitation, emphasizing external parts and excluding interior volumes.  
rdfs:seeAlso: https://www.wikidata.org/wiki/Q811979   
dcterms:modified: 2024-12-5  
dcterms:creator: Vittorio Lauro


E: Architectural element (part of an architectural structure)
https://photogrammetry.altervista.org/items/show/429 
All those elements that are part of an architectural structure (D) both structurally (such as pillars and bastions) and as parts of an external structure (windows, portals and doors).
Architectural elements may still be in place or may have been removed from the main structure or may never have been part of it.

rdfs:label: E (Architectural Element - Part of an Architectural Structure)  
skos:definition: Elements that are part of an architectural structure, both structurally (such as pillars and bastions) and as parts of external structure (windows, portals, and doors). These elements may still be in place or may have been removed from the main structure or never have been part of it.  
skos:altLabel: Architectural Element, Structural Element  
dcterms:source: PODS Thesaurus  
skos:scopeNote: Includes structural and decorative elements that form part of an architectural structure, with potential variations in their preservation or removal.  
owl:versionInfo: 1.0  
dcterms:description: Defines various parts of an architectural structure that may still be in place, removed, or never part of the main structure.  
rdfs:seeAlso:  http://vocab.getty.edu/page/aat/300000885  
dcterms:modified: 2024-12-5  
dcterms:creator: Vittorio Lauro 


F: Cave or underground structure
https://photogrammetry.altervista.org/items/show/430 
Caves, rooms and underground environments. Any finished practicable volume, including the environments that make up architectural structures 

rdfs:label: F (Cave or Underground Structure)  
skos:definition: Caves, rooms, and underground environments. Any finished practicable volume, including the environments that make up architectural structures.  
skos:altLabel: Underground Structure, Subterranean Environment  
dcterms:source: FOPPA Manual  
skos:scopeNote: Covers all types of underground spaces that are accessible or formed as part of architectural or archaeological environments.  
owl:versionInfo: 1.0  
dcterms:description: Refers to subterranean or cave-like structures that may be practical to access, including those that make up parts of larger architectural sites.  
rdfs:seeAlso: https://www.wikidata.org/wiki/Q35509, https://www.wikidata.org/wiki/Q44377, https://www.wikidata.org/wiki/Q172896     
dcterms:modified: 2024-12-5  
dcterms:creator: Vittorio Lauro  


G: Landscape element
https://photogrammetry.altervista.org/items/show/431 
Landscape elements such as plains, woods, clearings, cliffs and any landscape element derived from the action of nature and anthropic action but which cannot be traversed within it. A rock structure does not fall into this category, but rather the facade is an architectural structure (D) and its interior is a walkable volume (F). Dynamic or transforming landscape elements such as landslides, sinkholes, and sink holes also fall into this category. Elements of the landscape modified by human action but not visitable fall into this category. (So ​​Mount Rashmure does NOT fall into this category, the Behistun carvings do fall into this category).

rdfs:label: G (Landscape Element)  
skos:definition: Landscape elements such as plains, woods, clearings, cliffs, and any landscape element derived from the action of nature and anthropic action but which cannot be traversed within it. It also includes dynamic or transforming landscape elements such as landslides and sinkholes.  
skos:altLabel: Landscape Feature, Geographical Element  
dcterms:source: PODS Thesaurus  
skos:scopeNote: Refers to natural or modified landscape features that are significant but not traversable, including dynamic features shaped by natural or human actions.  
owl:versionInfo: 2.5  
dcterms:description: Describes landscape elements that are either natural or human-modified, not typically visitable or accessible.  
rdfs:seeAlso: https://www.wikidata.org/wiki/Q107425 , http://vocab.getty.edu/page/aat/300008631, http://vocab.getty.edu/page/aat/300435107 , http://vocab.getty.edu/page/aat/300008932 , http://vocab.getty.edu/page/aat/300419990 , 
dcterms:modified: 2024-12-5  
dcterms:creator: Vittorio Lauro 




Thesaurus for F18 Dominant Geometry Type
By dominant geometry we mean the geometry assumed by the conjunction of the opposite vertices of the object according to an approximation based on the inclination of the faces not exceeding 45 degrees. This distinction is necessary for the application of the "rule of opposites" as defined in the FOPPA Manual. For example, a basketball is a sphere, a bottle is a cylinder, a book is a parallelepiped, a κρατήρ is a bowl/hemisphere. As an approximation, however, we can say that an irregular glass bead is a sphere, a ceramic shard or an animal jaw is a parallelepiped, a column is a cylinder and a crater or a lake are hemisphere.
Sphere
https://photogrammetry.altervista.org/items/show/432 
A sphere is a perfectly round geometrical object in three-dimensional space, like a ball. Examples include a basketball or a glass bead.

rdfs:label: Sphere  
skos:definition: A sphere is a perfectly round geometrical object in three-dimensional space, such as a ball. Examples include a basketball or a glass bead.  
skos:altLabel: Round Object, Spherical Shape  
dcterms:source: FOPPA Manual  
skos:scopeNote: A geometric shape characterized by uniformity and symmetry in all directions.  
owl:versionInfo: 1.0  
dcterms:description: Describes a perfectly round geometrical shape, used to classify objects like basketballs and beads.  
rdfs:seeAlso: http://vocab.getty.edu/page/aat/300378898   
dcterms:modified: 2024-12-13  
dcterms:creator: Vittorio Lauro 

Parallelepiped
https://photogrammetry.altervista.org/items/show/433 

A parallelepiped is a six-faced figure (also called a polyhedron) where each face is a parallelogram. Examples include a book or a ceramic shard.

rdfs:label: Parallelepiped  
skos:definition: A parallelepiped is a six-faced figure (also called a polyhedron) where each face is a parallelogram. Examples include a book or a ceramic shard.  
skos:altLabel: Rectangular Object, Polyhedron  
dcterms:source: FOPPA Manual  
skos:scopeNote: A six-faced shape, where opposite faces are parallelograms, often used for objects with rectangular or angular properties.  
owl:versionInfo: 1.0  
dcterms:description: Describes a polyhedral object with six faces that are parallelograms, such as a book or ceramic shard.  
rdfs:seeAlso: https://www.wikidata.org/wiki/Q181658   
dcterms:modified: 2024-12-13  
dcterms:creator: Vittorio Lauro  

Hemisphere
https://photogrammetry.altervista.org/items/show/434 
A hemisphere is half of a sphere, typically divided by a plane passing through its center. Examples include a crater or a bowl.

rdfs:label: Hemisphere  
skos:definition: A hemisphere is half of a sphere, typically divided by a plane passing through its center. Examples include a crater or a bowl.  
skos:altLabel: Half-Sphere, Semi-Spherical Object  
dcterms:source: FOPPA Manual  
skos:scopeNote: A geometric shape representing half of a sphere, often used to describe objects like craters or bowls.  
owl:versionInfo: 1.0  
dcterms:description: A three-dimensional object that is half of a sphere, such as a crater or a bowl, divided by a plane.  
rdfs:seeAlso: https://www.wikidata.org/wiki/Q47091889    
dcterms:modified: 2024-12-13  
dcterms:creator: Vittorio Lauro  

Cylinder
https://photogrammetry.altervista.org/items/show/435 
A cylinder has two parallel circular bases connected by a curved surface. Examples include a column or a bottle.

rdfs:label: Cylinder  
skos:definition: A cylinder has two parallel circular bases connected by a curved surface. Examples include a column or a bottle.  
skos:altLabel: Cylindrical Object, Round Column  
dcterms:source: FOPPA Manual  
skos:scopeNote: A three-dimensional geometric shape with two parallel circular bases connected by a curved surface.  
owl:versionInfo: 1.0  
dcterms:description: Describes a geometric shape with two parallel circular faces and a curved side, such as columns or bottles.  
rdfs:seeAlso:  http://vocab.getty.edu/page/aat/300163037   
dcterms:modified: 2024-12-13 
dcterms:creator: Vittorio Lauro 

Plane Surface
https://photogrammetry.altervista.org/items/show/436 
A plane surface is a flat, two-dimensional surface extending infinitely in all directions. Examples include a flat stone tablet or a pavement segment.

rdfs:label: Plane Surface  
skos:definition: A plane surface is a flat, two-dimensional surface extending infinitely in all directions. Examples include a flat stone tablet or a pavement segment.  
skos:altLabel: Flat Surface, Two-Dimensional Plane  
dcterms:source: FOPPA Manual 
skos:scopeNote: A perfectly flat, two-dimensional surface that extends infinitely, commonly used in architecture and archaeology.  
owl:versionInfo: 1.0  
dcterms:description: A flat, two-dimensional surface found in various objects, such as stone tablets or pavement segments.  
rdfs:seeAlso: https://www.wikidata.org/wiki/Q17285  , https://www.wikidata.org/wiki/Q160091  , http://vocab.getty.edu/page/aat/300008805  
dcterms:modified: 2024-12-13 
dcterms:creator: Vittorio Lauro  

Irregular shape/Landscape
https://photogrammetry.altervista.org/items/show/437 
An irregular shape does not fit neatly into standard geometric categories and has uneven or asymmetrical surfaces. Examples include an irregular animal remains like Lyuba's mummy or a piece of pottery with an unusual form.

rdfs:label: Irregular Shape/Landscape  
skos:definition: An irregular shape does not fit neatly into standard geometric categories and has uneven or asymmetrical surfaces. Examples include irregular animal remains like Lyuba's mummy or a piece of pottery with an unusual form.  
skos:altLabel: Asymmetrical Shape, Non-Standard Geometry  
dcterms:source: FOPPA Manual 
skos:scopeNote: A shape that lacks symmetry or standard geometric form, often used to describe organic objects or irregular artifacts.  
owl:versionInfo: 1.0  
dcterms:description: Refers to shapes that do not fit into traditional geometric categories, such as irregular bones or unusual pottery.  
rdfs:seeAlso: http://vocab.getty.edu/page/aat/300010347, https://www.wikidata.org/wiki/Q107425  
dcterms:modified: 2024-12-13 
dcterms:creator: Vittorio Lauro  


Thesaurus for F155 Orientation of the 3D Model
The Orientation of the 3D Model Thesaurus is a structured vocabulary that categorizes terms describing the spatial positioning of 3D models in relation to reference systems. This thesaurus serves as a standard framework for documenting and communicating how 3D models are oriented within their coordinate systems, aiding researchers, archivists, and developers in digital heritage, archaeology, and engineering fields. By providing terms such as "Front-facing," "Top-oriented," and "Aligned to True North," it helps ensure consistency in metadata documentation across diverse projects. This thesaurus supports workflows involving comparative analysis, geospatial integration, and visualization by establishing a clear understanding of spatial relationships. The development of the thesaurus fills a critical gap in digital workflows, offering a semantic tool for enhancing interoperability and traceability of 3D datasets. It is particularly relevant for collaborative efforts where accurate spatial alignment is necessary for model integration, restoration projects, or computational analyses.

Reference Axes
AX
X-Axis Oriented: The model is oriented along the X-axis.
https://photogrammetry.altervista.org/items/show/438 

rdfs:label: X-Axis Oriented
skos:definition: The model is oriented along the X-axis of the coordinate system, aligning its primary orientation with the horizontal axis.
skos:altLabel: Aligned to X-Axis, Horizontal Orientation
dcterms:source: PODS Declaration
skos:scopeNote: Use this term when the model's primary orientation is aligned with the X-axis.
owl:versionInfo: 1.0
dcterms:description: Describes a spatial orientation where the model's primary alignment follows the X-axis of its coordinate reference system.
rdfs:seeAlso: 
:X_Axis_Orientation a geo:Geometry ;
    rdfs:label "X-Axis Oriented" ;
    geo:asWKT "POINT (1 0 0)"^^geo:wktLiteral ;
    rdfs:comment "The model is oriented along the X-axis." .


dcterms:modified: 2024-12-5
dcterms:creator: Vittorio Lauro


AY
Y-Axis Oriented: The model is oriented along the Y-axis.
https://photogrammetry.altervista.org/items/show/439 

rdfs:label: Y-Axis Oriented
skos:definition: The model is oriented along the Y-axis of the coordinate system, aligning its primary orientation with the vertical axis.
skos:altLabel: Aligned to Y-Axis, Vertical Orientation
dcterms:source: PODS Declaration
skos:scopeNote: Use this term when the model's primary orientation is aligned with the Y-axis.
owl:versionInfo: 1.0
dcterms:description: Describes a spatial orientation where the model's primary alignment follows the Y-axis of its coordinate reference system.
rdfs:seeAlso: 
:Y_Axis_Orientation a geo:Geometry ;
    rdfs:label "Y-Axis Oriented" ;
    geo:asWKT "POINT (0 1 0)"^^geo:wktLiteral ;
    rdfs:comment "The model is oriented along the Y-axis." .


dcterms:modified: 2024-12-5
dcterms:creator: Vittorio Lauro

AZ
Z-Axis Oriented: The model is oriented along the Z-axis.
https://photogrammetry.altervista.org/items/show/440 
rdfs:label: Z-Axis Oriented
skos:definition: The model is oriented along the Z-axis of the coordinate system, aligning its primary orientation with the depth axis.
skos:altLabel: Aligned to Z-Axis, Depth Orientation
dcterms:source: PODS Declaration
skos:scopeNote: Use this term when the model's primary orientation is aligned with the Z-axis.
owl:versionInfo: 1.0
dcterms:description: Describes a spatial orientation where the model's primary alignment follows the Z-axis of its coordinate reference system.
rdfs:seeAlso: 

:Z_Axis_Orientation a geo:Geometry ;
    rdfs:label "Z-Axis Oriented" ;
    geo:asWKT "POINT (0 0 1)"^^geo:wktLiteral ;
    rdfs:comment "The model is oriented along the Z-axis." .


dcterms:modified: 2024-12-5
dcterms:creator: Vittorio Lauro



Rotations
NR
No Rotation: No rotation applied (model aligned to the global system).
https://photogrammetry.altervista.org/items/show/441 
rdfs:label: No Rotation  
skos:definition: Indicates that no rotation has been applied to the model, aligning it with the global coordinate system.  
skos:altLabel: Unrotated, Global Alignment  
dcterms:source: PODS Declaration  
skos:scopeNote: Use this term when the model retains its original alignment without any applied rotational transformations.  
owl:versionInfo: 1.0  
dcterms:description: Describes a model that has not undergone rotational adjustments, maintaining its alignment with the global system.  
rdfs:seeAlso: 
:No_Rotation a geo:Geometry ;
    rdfs:label "No Rotation" ;
    skos:definition "Indicates that no rotation has been applied to the model, aligning it with the global coordinate system." ;
    geo:asWKT "POINT (0 0 0)"^^geo:wktLiteral ;
    rdfs:comment "The model is aligned with the global coordinate system without rotation." .

 
dcterms:modified: 2024-12-5  
dcterms:creator: Vittorio Lauro 

RZ
Yaw Rotation: Rotation around the Z-axis (horizontal angle).

rdfs:label: Yaw Rotation
skos:definition: Rotation of the model around the Z-axis, altering its horizontal orientation within the coordinate system.
skos:altLabel: Horizontal Rotation, Rotation Around Z-Axis
dcterms:source: PODS Declaration
skos:scopeNote: Apply this term to describe models rotated horizontally relative to their global coordinate system.
dcterms:description: Specifies the rotation of a 3D model along the horizontal plane, modifying its orientation relative to a reference axis.
rdfs:seeAlso: 

:Yaw_Rotation a geo:Geometry ;
    rdfs:label "Yaw Rotation" ;
    skos:definition "Rotation of the model around the Z-axis, altering its horizontal orientation within the coordinate system." ;
    geo:asWKT "POINT (0 0 1)"^^geo:wktLiteral ;
    rdfs:comment "The model has been rotated around the Z-axis, affecting its horizontal orientation." .


dcterms:modified: 2024-12-5
dcterms:creator: Vittorio Lauro


RY
Pitch Rotation: Rotation around the Y-axis (vertical angle).
https://photogrammetry.altervista.org/items/show/442 
rdfs:label: Pitch Rotation  
skos:definition: Rotation of the model around the Y-axis, altering the vertical angle of the object.  
skos:altLabel: Rotation on Y-axis, Vertical Rotation  
skos:broader: Rotations  
skos:related: Roll Rotation, Yaw Rotation  
dcterms:identifier: RY  
dcterms:source: PODS Declaration  
dcterms:language: en  
skos:scopeNote: Use this term to describe vertical angular adjustments of the model along the Y-axis.  
owl:versionInfo: 1.0  
dcterms:status: Approved  
dcterms:description: Defines the model's rotation around its vertical Y-axis, typically used for tilting adjustments.  
rdfs:seeAlso:

:Pitch_Rotation a geo:Geometry ;
    rdfs:label "Pitch Rotation" ;
    skos:definition "Rotation of the model around the Y-axis, altering the vertical angle of the object." ;
    geo:asWKT "POINT (0 1 0)"^^geo:wktLiteral ;
    rdfs:comment "The model has been rotated around the Y-axis, affecting its vertical angle." .

  
skos:inScheme: Orientation of the 3D Model Thesaurus  
dcterms:created: 2024-11-25  
dcterms:modified: 2024-12-5  
dcterms:creator: Vittorio Lauro

RX
Roll Rotation: Rotation around the X-axis (longitudinal angle).
https://photogrammetry.altervista.org/items/show/443 
rdfs:label: Roll Rotation  
skos:definition: Rotation of the model around the X-axis, altering its longitudinal orientation.  
skos:altLabel: Rotation on X-axis, Longitudinal Rotation  
dcterms:source: PODS Declaration  
skos:scopeNote: Use this term to describe adjustments made by rolling the model along the X-axis.  
owl:versionInfo: 1.0  
dcterms:description: Refers to the rotation of the model along its longitudinal axis, typically used for rolling transformations.  
rdfs:seeAlso: 

:Roll_Rotation a geo:Geometry ;
    rdfs:label "Roll Rotation" ;
    skos:definition "Rotation of the model around the X-axis, altering its longitudinal orientation." ;
    geo:asWKT "POINT (1 0 0)"^^geo:wktLiteral ;
    rdfs:comment "The model has been rotated around the X-axis, affecting its longitudinal orientation." .

 
dcterms:modified: 2024-12-5  
dcterms:creator: Vittorio Lauro 


Global Orientation
NF
North-Facing: The model is oriented towards the true North.
https://photogrammetry.altervista.org/items/show/444 
rdfs:label: North-Facing
skos:definition: The model is oriented towards the true North, aligning its primary axis with the geographic North direction.
skos:altLabel: Aligned to North, Oriented to True North
dcterms:source: PODS Declaration
skos:scopeNote: Use this term to describe models oriented to align their axis with the North in a geospatial reference.
owl:versionInfo: 1.0
dcterms:description: Indicates a 3D model whose primary alignment corresponds to the geographic North.
rdfs:seeAlso: 

:North_Facing a geo:Geometry ;
    rdfs:label "North-Facing" ;
    skos:definition "The model is oriented towards the true North, aligning its primary axis with the geographic North direction." ;
    geo:asWKT "POINT (0 1 0)"^^geo:wktLiteral ;
    rdfs:comment "The model is oriented towards the true North, with the primary axis pointing in the North direction." .


dcterms:modified: 2024-12-5
dcterms:creator: Vittorio Lauro

SF
South-Facing: The model is oriented towards the true South.
https://photogrammetry.altervista.org/items/show/445 
rdfs:label: South-Facing  
skos:definition: Indicates that the model is oriented towards the true South.  
skos:altLabel: Facing South, Oriented Southward  
dcterms:source: PODS Declaration  
skos:scopeNote: Use this term to describe models positioned or aligned with the true South direction in a global reference system.  
owl:versionInfo: 1.0  
dcterms:description: Defines the alignment of the model where its primary orientation is towards the South within a global georeferencing framework.  
rdfs:seeAlso: 

:South_Facing a geo:Geometry ;
    rdfs:label "South-Facing" ;
    skos:definition "Indicates that the model is oriented towards the true South." ;
    geo:asWKT "POINT (0 -1 0)"^^geo:wktLiteral ;
    rdfs:comment "The model is oriented towards the true South." .

 
dcterms:modified: 2024-12-5  
dcterms:creator: Vittorio Lauro  

EF
East-Facing: The model is oriented towards the East.
https://photogrammetry.altervista.org/items/show/446 
rdfs:label: East-Facing  
skos:definition: Indicates that the model is oriented towards the East.  
skos:altLabel: Facing East, Oriented Eastward  
dcterms:source: PODS Declaration  
skos:scopeNote: Use this term to describe models positioned or aligned with the East direction in a global reference system.  
owl:versionInfo: 1.0  
dcterms:description: Defines the alignment of the model where its primary orientation is towards the East within a global georeferencing framework.  
rdfs:seeAlso: 
 
:East_Facing a geo:Geometry ;
    rdfs:label "East-Facing" ;
    skos:definition "Indicates that the model is oriented towards the East." ;
    geo:asWKT "POINT (1 0 0)"^^geo:wktLiteral ;
    rdfs:comment "The model is oriented towards the East." .


dcterms:modified: 2024-12-5  
dcterms:creator: Vittorio Lauro  

WF
West-Facing: The model is oriented towards the West.
https://photogrammetry.altervista.org/items/show/447 
rdfs:label: West-Facing  
skos:definition: Indicates that the model is oriented towards the West.  
skos:altLabel: Facing West, Oriented Westward  
dcterms:source: PODS Declaration  
skos:scopeNote: Use this term to describe models positioned or aligned with the West direction in a global reference system.  
owl:versionInfo: 1.0  
dcterms:description: Defines the alignment of the model where its primary orientation is towards the West within a global georeferencing framework.  
rdfs:seeAlso:


:West_Facing a geo:Geometry ;
    rdfs:label "West-Facing" ;
    skos:definition "Indicates that the model is oriented towards the West." ;
    geo:asWKT "POINT (-1 0 0)"^^geo:wktLiteral ;
    rdfs:comment "The model is oriented towards the West." .

  
dcterms:modified: 2024-12-5  
dcterms:creator: Vittorio Lauro  


Relative Orientation
OGP
Relative to Ground Plane: The model is aligned with the ground plane (for example, with a flat surface that coincides with the XY plane).
https://photogrammetry.altervista.org/items/show/448 
rdfs:label: Relative to Ground Plane
skos:definition: The model is aligned with the ground plane, such that its base coincides with the XY plane of the reference system.
skos:altLabel: Aligned with Ground, XY-Plane Aligned
dcterms:source: PODS Declaration
skos:scopeNote: Use this term for models oriented so that their base aligns with a flat horizontal plane.
owl:versionInfo: 1.0

dcterms:description: Describes the spatial alignment of a model relative to a horizontal reference plane.
rdfs:seeAlso: 

:Relative_to_Ground_Plane a geo:Geometry ;
    rdfs:label "Relative to Ground Plane" ;
    skos:definition "The model is aligned with the ground plane, such that its base coincides with the XY plane of the reference system." ;
    geo:asWKT "POLYGON ((0 0, 1 0, 1 1, 0 1, 0 0))"^^geo:wktLiteral ;
    rdfs:comment "The model is aligned with the ground plane, typically represented by the XY plane of the reference system." .


dcterms:modified: 2024-11-25
dcterms:creator: Vittorio Lauro

OOF
Relative to Object Features: Orientation based on specific features of the object, such as a leading edge or prominent detail.
https://photogrammetry.altervista.org/items/show/449 
rdfs:label: Relative to Object Features  
skos:definition: Orientation based on specific features of the object, such as a leading edge or prominent detail.  
skos:altLabel: Object-Feature Alignment, Feature-Based Orientation  
dcterms:source: PODS Declaration  
skos:scopeNote: Use this term when the orientation of the model is determined by specific features or details of the object itself, aiding in accurate alignment or presentation.  
owl:versionInfo: 1.0  
dcterms:description: Defines the spatial alignment of a 3D model relative to distinct features of the object, ensuring precision in documentation and visualization workflows.  
rdfs:seeAlso: 

:Relative_to_Object_Features a geo:Geometry ;
    rdfs:label "Relative to Object Features" ;
    skos:definition "Orientation based on specific features of the object, such as a leading edge or prominent detail." ;
    geo:asWKT "LINESTRING (0 0, 1 1)"^^geo:wktLiteral ;
    rdfs:comment "The model is oriented based on specific features of the object, like a leading edge or other prominent features." .

  
 
dcterms:modified: 2024-11-25  
dcterms:creator: Vittorio Lauro  

OAM
Aligned with Another Model: The model is oriented with respect to another model (for example, a point cloud or reference model).
https://photogrammetry.altervista.org/items/show/450 
rdfs:label: Aligned with Another Model  
skos:definition: The model is oriented with respect to another model, such as a point cloud or reference model.  
skos:altLabel: Model-to-Model Alignment, Comparative Model Orientation  
dcterms:source: PODS Declaration  
skos:scopeNote: Use this term to describe models that are spatially oriented in relation to another model, facilitating comparative analysis or integration in digital heritage workflows.  
owl:versionInfo: 1.0  
dcterms:description: Defines the orientation of a 3D model in reference to another model, ensuring interoperability and coherence in multi-model projects.  
rdfs:seeAlso: 

:Aligned_with_Another_Model a geo:Geometry ;
    rdfs:label "Aligned with Another Model" ;
    skos:definition "The model is oriented with respect to another model, such as a point cloud or reference model." ;
    geo:asWKT "MULTILINESTRING ((0 0, 2 2), (2 2, 3 3))"^^geo:wktLiteral ;
    rdfs:comment "The model is aligned with another model, such as a point cloud or reference model." .

 
dcterms:modified: 2024-11-25  
dcterms:creator: Vittorio Lauro 


Symmetry Specifications
SO
Symmetrical Orientation: The model is oriented so that the intrinsic symmetry of the object is respected.
https://photogrammetry.altervista.org/items/show/451 
rdfs:label: Symmetrical Orientation  
skos:definition: The model is oriented so that the intrinsic symmetry of the object is respected.  
skos:altLabel: Symmetry-Preserving Orientation, Balanced Orientation  
dcterms:source: PODS Declaration  
skos:scopeNote: Use this term when the 3D model's orientation respects the inherent symmetrical properties of the object, ensuring an accurate representation of its geometry.  
owl:versionInfo: 1.0  
dcterms:description: Defines an orientation in which the model is aligned to maintain its intrinsic symmetry, aiding in visualization, analysis, and comparison.  
rdfs:seeAlso:  none
dcterms:modified: 2024-11-25  
dcterms:creator: Vittorio Lauro  

AO
Asymmetrical Orientation: The orientation does not respect the symmetry of the object.
Perspective or View Specifications
https://photogrammetry.altervista.org/items/show/452 
rdfs:label: Asymmetrical Orientation  
skos:definition: The orientation does not respect the symmetry of the object.  
skos:altLabel: Symmetry-Ignoring Orientation, Unbalanced Orientation  
dcterms:source: PODS Declaration  
skos:scopeNote: Use this term when the 3D model's orientation intentionally disregards the object's symmetry, often to highlight specific features or align with external criteria.  
owl:versionInfo: 1.0  
dcterms:description: Defines an orientation in which the model is deliberately aligned without maintaining its inherent symmetry, supporting use cases requiring unconventional perspectives or alignments.  
rdfs:seeAlso:  
dcterms:modified: 2024-11-25  
dcterms:creator: Vittorio Lauro  



Perspective or View Specifications
VT
Top-Down View: The model is oriented for a top view.
https://photogrammetry.altervista.org/items/show/453 
rdfs:label: Top-Down View
skos:definition: The model is oriented to present a top view, allowing the user to observe it from above.
skos:altLabel: Overhead View, Bird’s Eye View
dcterms:source: PODS Declaration
skos:scopeNote: This orientation is useful for visualizing the layout or distribution of features from above.
owl:versionInfo: 1.0
dcterms:description: Indicates that the 3D model is presented with an overhead perspective for analysis or visualization.
rdfs:seeAlso: 

:Top_Down_View a owl:Class ;
    rdfs:label "Top-Down View" ;
    skos:definition "The model is oriented to present a top view, allowing the user to observe it from above." ;
    geo:geometry [ geo:asWKT "POINT(0 0)"^^geo:wktLiteral ;  # Example coordinates for the camera position
                  geo:hasOrientation "90"^^xsd:decimal ] ; # Example of top-down orientation angle (view from above).


dcterms:modified: 2024-11-25
dcterms:creator: Vittorio Lauro

VF
Front View: The model is oriented for a front view.
https://photogrammetry.altervista.org/items/show/454 
rdfs:label: Front View  
skos:definition: The model is oriented for a front view.  
skos:altLabel: Frontal Orientation, Forward View  
dcterms:source: PODS Declaration  
skos:scopeNote: Use this term to describe the orientation of the model when it is displayed from the front-facing perspective, highlighting the primary façade or forward-facing details.  
owl:versionInfo: 1.0  
dcterms:description: Defines the orientation of a 3D model in which the front-facing portion is prioritized, aiding in visual clarity for educational or presentational purposes.  
rdfs:seeAlso: 

:Front_View a owl:Class ;
    rdfs:label "Front View" ;
    skos:definition "The model is oriented for a front view." ;
    geo:geometry [ geo:asWKT "POINT(0 0)"^^geo:wktLiteral ;  # Example coordinates for the camera position
                  geo:hasOrientation "0"^^xsd:decimal ] ; # Example of front-facing orientation angle (view from the front).

 
dcterms:modified: 2024-11-25  
dcterms:creator: Vittorio Lauro

VS
Side View: The model is oriented for a side view (left or right).
https://photogrammetry.altervista.org/items/show/455 
rdfs:label: Side View  
skos:definition: The model is oriented for a side view (left or right).  
skos:altLabel: Lateral View, Profile Orientation  
dcterms:source: PODS Declaration  
skos:scopeNote: Use this term when the model is oriented to display a profile or side perspective, often used to highlight structural or design details.  
owl:versionInfo: 1.0  
dcterms:description: Defines the orientation of a 3D model from a lateral or side angle, providing insights into the object’s profile and side features.  
rdfs:seeAlso: 

:Side_View a owl:Class ;
    rdfs:label "Side View" ;
    skos:definition "The model is oriented for a side view (left or right)." ;
    geo:geometry [ geo:asWKT "POINT(0 0)"^^geo:wktLiteral ;  # Example coordinates for the camera position
                  geo:hasOrientation "90"^^xsd:decimal ] ; # Example of side view orientation (either left or right).

 
dcterms:modified: 2024-11-25  
dcterms:creator: Vittorio Lauro  

VI
Isometric View: The model is oriented for an isometric view (associated with 3D graphics and CAD).
https://photogrammetry.altervista.org/items/show/456 
rdfs:label: Isometric View  
skos:definition: The model is oriented for an isometric view (associated with 3D graphics and CAD).  
skos:altLabel: 3D Perspective View, CAD Isometric View  
dcterms:source: PODS Declaration  
skos:scopeNote: Use this term to describe the orientation of the model when displayed in an isometric projection, often used in 3D design and technical documentation.  
owl:versionInfo: 1.0  
dcterms:description: Defines the orientation of a 3D model in an isometric perspective, enabling a balanced, three-dimensional view without distortion from perspective scaling.  
rdfs:seeAlso: 

:Isometric_View a owl:Class ;
    rdfs:label "Isometric View" ;
    skos:definition "The model is oriented for an isometric view (associated with 3D graphics and CAD)." ;
    geo:geometry [ geo:asWKT "POINT(0 0)"^^geo:wktLiteral ;  # Example coordinates for the camera position
                  geo:hasOrientation "45"^^xsd:decimal ] ; # Example of isometric view orientation angle (45-degree angle typical for isometric views).

 
dcterms:modified: 2024-11-25  
dcterms:creator: Vittorio Lauro  





Metadata legitimacy standards

In the context of the PODS research framework, we encountered a critical challenge in defining a qualitative and legitimacy-based scale for evaluating 3D models. The difficulty lies in the impracticality of using an absolute numerical parameter, as numerical values can convey vastly different meanings depending on the specific context. For instance, a 3D model with one million points may be highly detailed when representing a ceramic fragment but insufficient when modeling a large castle wall. Moreover, the numerical point count alone does not indicate the quality or accuracy of the model, as densification techniques might artificially inflate point numbers, leading to non-representative data that does not accurately reflect the physical object.

Given this context, and the variability in data produced by different photogrammetric or scanning devices, our approach shifted from quantitative metrics to an assessment based on the final intended purpose of the 3D model. Instead of evaluating a model’s legitimacy through absolute values, we propose a binary system where the presence or absence of specific metadata entries determines the model's usability for its designated purpose. This approach emphasizes metadata fields essential for verifying the model's reliability in specific applications, rather than relying on quantitative measures alone.

Currently, we have identified four main final purposes for a 3D model, organized within a hierarchical framework of Metadata Legitimacy Standards. Each level builds upon the previous, creating a cumulative structure where metadata requirements are progressively inclusive. This structure is as follows:

- Teaching and Dissemination: If the metadata of a 3D model includes all classes marked as essential for “teaching and dissemination,” the model is deemed suitable for educational and dissemination purposes.
- Conservation and Enhancement: If, in addition to the metadata required for teaching and dissemination, the model includes all classes necessary for “conservation and enhancement,” then the model can also be used for preservation purposes.
- Archaeometric Analysis: If, building upon the previous levels, the model includes all metadata classes necessary for “archaeometric analysis,” it is then deemed suitable for scientific or analytical purposes, allowing it to support precise measurements and research applications.
- Restoration Analysis: Finally, if the metadata satisfies all classes designated for “restoration analysis,” alongside those required for the previous categories, the model is considered suitable for use in restoration planning and analysis.

Classes designated with `dc:description "Relevant for:" Contextual Objectives` address metadata specific to particular, context-dependent objectives, thus allowing the metadata framework to adapt to various specialized requirements.

This hierarchy of Metadata Legitimacy Standards represents a preliminary solution to the issue of model legitimacy assessment within the PODS framework. This structure is currently conceptualized as an initial answer to our research question, providing a foundation for further development. Future work will seek to refine this binary-based framework, introducing more sophisticated metrics and perhaps nuanced gradations within each purpose category. Through continued research, we aim to establish a more robust methodology for 3D model evaluation, one that better accounts for both quantitative and qualitative aspects of metadata while adapting to the unique requirements of different cultural heritage contexts.




