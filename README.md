PODS 1_1_7

Protocol of Ontological Digital Survey 

Introduction to the PODS Ontology 

The Protocol of Ontological Digital Survey (PODS) is an ontology designed to standardize and formalize the digital surveying process, particularly for the documentation and preservation of cultural heritage. Developed as a refinement and expansion of previous protocols such as BeAPG and FOPPA, PODS focuses on the precise metadata representation of each step in the digital surveying workflow, ensuring a structured and semantically coherent approach to 3D data acquisition, processing, and management.

The ontology integrates established standards such as SKOS, QUDT, and CIDOC-CRM, with specific extensions like CIDOC-CRMdig, to enhance interoperability and compatibility with international data-sharing platforms, including Wikimedia’s database structures. PODS provides a robust framework for representing the phases, sub-phases, actions, and tools involved in digital surveying, facilitating the creation of accurate, structured data about three-dimensional cultural heritage assets.

The ontology is organized into classes and properties that define and describe the key components of the digital surveying process. These classes capture essential information about the objects, processes, and tools used in 3D photogrammetry, enabling the precise cataloging of digital models, point clouds, and related metadata. PODS aims to create a scalable, adaptable system that can be applied in diverse contexts, from archaeological excavation sites to museum digitalization projects.

This document presents the detailed structure of the PODS ontology, outlining each class and its associated properties, along with their relationships to established standards. The goal is to provide a clear and systematic framework that ensures consistency, accuracy, and completeness in digital heritage documentation.




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
Survey Object denotes any object subjected to photogrammetric surveying or any kind of digital surveying. It represents the target of data acquisition processes, crucial for generating detailed digital records, analyses, and reconstructions within the FOPPA model for archaeological documentation. It must be a solid and visible object. The expression visible means that it interacts with light.
Examples:
a wild boar jaw AFMNM005 detected with photogrammetric technique at the laboratory of the archaeological museum of Okayama (Japan) coming from the Minamikata excavation in the context of the BeArchaeo project (Lauro, 2019)
A castle surveyed with photogrammetric technique (Artopoulos 2015)
A fresco in a medieval chapel (D. Abate 2016)

Label: SurveyObject



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

—-------------------------------------------------------------------------------------------

F5 Exporting
URI: https://photogrammetry.altervista.org/items/show/91 
SubClass of CIDC-CRM class
D7 Digital Machine Event 
Scope Note 
Exporting involves the final stages of digital asset management. This phase encompasses exporting the processed data and archiving it for long-term preservation, ensuring the integrity and accessibility of digital records.
Examples:


Label: Exporting

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


—-------------------------------------------------------------------------------------------

F15 Recontruction Method 
URI: https://photogrammetry.altervista.org/items/show/101 
SubClass of: 
E29 Design and Procedure
Scope Note:
The Reconstruction Method class refers to the procedures and algorithms used to transform a densified point cloud into a polygonal mesh, thereby creating a structured 3D representation of an object or scene. This process involves generating polygons, typically triangles or quads, that form the mesh surface based on the spatial data from the point cloud. The Reconstruction Method also includes steps like mesh optimization, hole filling, and refinement to improve accuracy and ensure the continuity of the 3D surface. Different software solutions and algorithms such as Poisson Surface Reconstruction, Delaunay Triangulation, or Ball-Pivoting Algorithm are examples of methods employed during this phase.
Examples:
Applying the Poisson Surface Reconstruction algorithm in Metashape to create a high-fidelity mesh from a dense point cloud.
Using Delaunay Triangulation to generate a watertight 3D mesh in Zephyr from a multi-view photogrammetric survey.
Label: Modelling_ReconstructionMethod


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



—-------------------------------------------------------------------------------------------

F19 Scale Type 
URI: https://photogrammetry.altervista.org/items/show/105 
SubClass of: 
E55 Type
Scope Note:
The Scale Type class pertains to the classification of the size of an object according to various available thesauri. This classification reflects the volume of the object and, depending on the thesaurus employed, may also relate to its functional characteristics. This class serves as a basis for understanding the object's scale in relation to its volume and, when applicable, its function according to the selected thesaurus.
Examples: 
Small Object: Equal to or smaller than 1 cm (FOPPA).
Medium Object: Ranging from 1 cm to 30 cm (FOPPA)
Open Architectural Structure: Entire buildings or significant structures (FOPPA).
Bend (COSCHKR)
Corner  (COSCHKR)
Joint  (COSCHKR)
Label: AcquisitionScaleObjectType

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


—-------------------------------------------------------------------------------------------

F24  Texturing Type 
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



—-------------------------------------------------------------------------------------------

F27 Densified Point Cloud 
URI: https://photogrammetry.altervista.org/items/show/113 
SubClass of: 
D9 Data Object
Scope Note:
The Densified Point Cloud class refers to a refined set of three-dimensional data points that have undergone an additional processing stage to enhance point density. This process occurs independently from the initial matching phase and results in a more detailed representation of the object's surface geometry. Densified point clouds are crucial for improving the accuracy and quality of subsequent modeling and visualization tasks.

Examples:
A point cloud obtained after applying algorithms that increase the density of points to capture finer details of an archaeological site.
Densified point data generated from a laser scanner, where additional points are added to improve spatial resolution.
A processed point cloud used for advanced analysis and 3D reconstruction, characterized by a higher density of points compared to the initial output.
Enhanced point cloud data created through interpolation techniques to fill gaps in the original point set.
Label: ProcessedDensifiedPointCloud



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

—-------------------------------------------------------------------------------------------

F31 Processing Software
URI: https://photogrammetry.altervista.org/items/show/117 
SubClass of: 
D14 Software
Scope Note:
The Processing Software class refers to software specifically used to process raw data into point clouds and densified point clouds during the 3D modeling workflow. This software transforms the data acquired during the acquisition phase (e.g., images from photogrammetry or raw point clouds from laser scanning) and applies algorithms to generate an initial point cloud, followed by densification processes to refine and enrich the dataset. Processing Software is responsible for tasks such as matching, densification, and initial 3D reconstruction steps, ultimately laying the foundation for later stages of modeling.
Examples:
Software that processes photogrammetric images into an initial sparse point cloud and subsequently applies densification algorithms.
A 3D laser scanner’s companion software that converts raw scan data into a structured point cloud and performs densification.
LiDAR processing software that translates raw light detection and ranging data into a detailed and accurate point cloud.
Applications like Agisoft Metashape, RealityCapture, or Pix4D used to convert raw photogrammetry images into dense point clouds suitable for 3D modeling.
Label: ProcessingSoftware

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

—-------------------------------------------------------------------------------------------

F40 Eydotipe  
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

—-------------------------------------------------------------------------------------------

F42 Place Of Acquisition    
URI: https://photogrammetry.altervista.org/items/show/128 
SubClass of: 
E53 Place
Scope Note:
The Place of Acquisition class refers to the physical space where the acquisition took place, encompassing the location where the acquisition occurred or where the architectural structure that was surveyed is situated. This class is essential for contextualizing the data collected during the acquisition process and provides information on the geographical and cultural relevance of the acquired data.
Examples:
An archaeological site, such as the ruins of an ancient temple, identified as the Place of Acquisition for the photogrammetric survey.
A historic building, like a medieval castle, where the acquisition was performed, serving as the Place of Acquisition.
A landscape feature, such as a valley or a mountain, where the acquisition took place, denoting its significance in geographical studies.
An urban area, like a city square, where multiple structures were surveyed, specified as the Place of Acquisition.
Label: AcquisitionLocation

—-------------------------------------------------------------------------------------------

F43 Survey Date     
URI: https://photogrammetry.altervista.org/items/show/129 
SubClass of: 
E52 Time Span
Scope Note:
The Survey Date class refers to the time period expressed as a specific date when the survey was conducted. This class is crucial for documenting the temporal context of the acquisition process and allows for the establishment of a chronological framework for the collected data.
Examples:
The exact date when a photogrammetric survey was performed at a historic site, such as June 15, 2022.
The period during which an archaeological excavation took place, marked with specific survey dates for different phases of the project.
A timeframe noted for monitoring environmental changes, indicating survey dates for repeated assessments at a particular location.
The date assigned to a structural survey conducted on a bridge to evaluate its condition, such as March 1, 2023.
Label: AcquisitionDate

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

—-------------------------------------------------------------------------------------------

F45  Acquisition Coordinates 
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


—-------------------------------------------------------------------------------------------

F46  Matching
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

—-------------------------------------------------------------------------------------------


F47  Densification
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

—-------------------------------------------------------------------------------------------

F53 Dense Point Cloud Number of Point 
URI: https://photogrammetry.altervista.org/items/show/139 
SubClass of: 
E54 Dimension
Scope Note:
The Dense Point Cloud Number of Point class refers to the specific dimension that indicates the number of points in a densified point cloud (F27 Densified Point Cloud). This class records the total count of points generated after the densification process, offering crucial data about the granularity and density of the final point cloud used for 3D modeling and analysis.

Examples:

A dense point cloud of a scanned monument containing 15 million points.
Label: ProcessedDensePointCloudNumberOfPoint
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
—-------------------------------------------------------------------------------------------

F55 Depth Noise Filtering
URI: https://photogrammetry.altervista.org/items/show/141 
SubClass of: E13 Attribute Assignment

Scope Note:
The Depth Noise Filtering class refers to the assignment of depth noise reduction techniques or parameters applied to densified point clouds (F27 Densified Point Cloud). This class captures the process of identifying and filtering out noise, errors, or inaccuracies in the depth values of a point cloud. These filtering operations are particularly necessary in dense datasets where inaccuracies can affect the quality and reliability of subsequent reconstructions.

Examples:
In the densiefied point cloud of AFMNM005 the Depth Noise Filtering is Adaptive feature extraction -AFE-, gradient field estimation -GFE- and further accelerated gradient ascent -FAGA- (Lauro 2019)

Label: DensificationAttributeDepthNoiseFiltering
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
---------------------------------------------------------------------------

F100 3D Digital Twin 
URI: https://photogrammetry.altervista.org/items/show/145 
SubClass of: 
D9 Data Object
Scope Note:
The 3D Digital Twin class refers to the ultimate 3D model resulting from the complete acquisition and processing workflow. This model may be the outcome of either the F5 Exporting process or F4 Modelling, depending on the workflow followed. At this stage, the model is considered complete and will not undergo any further modifications. It is the final product that represents the culmination of all previous acquisition, processing, and modeling efforts, encapsulating all the geometric and textural information. This final model is typically used for documentation, analysis, visualization, or presentation purposes in various fields such as cultural heritage, architecture, and archaeology.
Examples:
The digital twin of the boar jaw preserved at the Okayama archaeological museum and signed as AF005MNM (Lauro 2019).
The digital twin of the excavation section of the Gobelki Tepe site (Polat 2020)
The digital twin of the no longer existing Bayman Buddhas (Gruen 2004).
Label: TridimensionalDigitalTwin
---------------------------------------------------------------------------

F59 Digital Scale  
URI: https://photogrammetry.altervista.org/items/show/146 
SubClass of: 
E54 Dimension
Scope Note:
The Digital Scale class refers to the scale of the 3D Digital Twin (F100), specifically in relation to the actual size of the object being represented. It indicates the proportional relationship between the dimensions of the digital model and the real-world measurements of the original object. This scale can be expressed in various formats, such as 1:1, 1:20, or other ratios, depending on how the 3D model has been created or intended to be used. The Digital Scale is crucial for accurate representation, visualization, and analysis, ensuring that the digital twin correctly reflects the physical dimensions of the object it represents.
Examples:
A digital scale of 1:1 for a final 3D model of a sculpture, indicating that the model is an exact replica of the original size.
A digital scale of 1:50 for an architectural model, showing that the digital representation is 50 times smaller than the actual building.
Label: TridimensionalDigitalTwin_DigitalScale
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
Label: 
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
---------------------------------------------------------------------------

F62 Texture Set of 3D Mesh
URI: https://photogrammetry.altervista.org/items/show/149 
SubClass of: 
D9 Data Object
Scope Note:
The Texture Set of 3D Mesh class refers to the collection of textures, which can be either singular or multiple, that are associated with a Textured 3D Mesh (F29). This class encompasses all the visual information applied to the 3D model's surface, which may include different texture maps such as diffuse, specular, normal, and bump maps. The texture set is crucial for enhancing the realism of the 3D model, providing detailed surface characteristics and visual cues that represent the physical properties of the object being modeled.
Examples:

A texture set consisting of a diffuse map, a normal map, and a specular map used to create a realistic surface appearance for a 3D model of a stone wall.
A collection of multiple textures applied to different parts of a 3D character model, including skin texture, clothing texture, and accessory texture, to achieve a rich and detailed visual representation.
Label: ProcessedTexturedMeshTextureSet
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
---------------------------------------------------------------------------

F64 Modelling Description 
URI: https://photogrammetry.altervista.org/items/show/151 
SubClass of: 
E62 String

Scope Note:
The Modelling Description class refers to a prose description of the modelling operations performed on a Textured Mesh (F29) within the context of Modelling (F4). This description provides a narrative account of the changes and modifications made to the 3D model, detailing the techniques, tools, and processes employed during the modelling phase. Such descriptions are essential for documentation purposes, allowing users to understand the adjustments made and the rationale behind them.
A description is distinguished from the information already established by other classes as it represents a string where elements not already classified can be annotated and allows a free annotation of information that can help guide the creation of new classes for the ontology.

Examples:

A description detailing how the texture was adjusted to enhance realism by applying a specific smoothing filter and how additional vertices were added to refine the model's geometry.
The string "elimination of the elements of the table and the set and focus on the find " in the context of modeling the 3D model of AF005MNM (Lauro 2019)
Label: Modelling_ModifyingDescription
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

---------------------------------------------------------------------------

F71 Final Use of Digital Twin
URI: https://photogrammetry.altervista.org/items/show/158 
SubClass of: 
D7 Digital Machine Event
Scope Note:
The Final Use of Digital Twin class refers to the final preparations and operations performed on the Digital Twin in accordance with the project's requirements. This class encompasses the generation of all necessary variants of the Digital Twin tailored for specific purposes, ensuring that the final outputs meet the intended application, whether for visualization, simulation, or analysis.

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
The 3D Model Video Rendering class refers to the output generated by rendering a 3D model into a video format. This video can be utilized for various purposes, such as presentations, educational demonstrations, or promotional content. The rendering process involves creating a visual representation of the 3D model in motion, showcasing its features, textures, and overall design.

Examples:

A video showcasing the architectural model of a building, rendered to highlight its design elements for a client presentation.
An educational video demonstrating the features of a historical artifact through 3D rendering.
Label: Exported3DModelVideoRendering
---------------------------------------------------------------------------

F73 Editing Video
URI: https://photogrammetry.altervista.org/items/show/160 
SubClass of: 
D7 Digital Machine Event
Scope Note:
The Editing Video class refers to the actions performed on the rendered video of the 3D model to modify, enhance, or refine its content. This includes tasks such as cutting, splicing, adding effects, and incorporating audio, all aimed at improving the final presentation quality of the video.

Examples:

Cutting segments of the 3D rendering video to create a more concise presentation for a seminar.
Adding background music and transitions to the video of a 3D model for promotional purposes.
Label: Exporting_EditingRenderingVideo
---------------------------------------------------------------------------

F74 Video Editing Software
URI: https://photogrammetry.altervista.org/items/show/161 
SubClass of: 
D14 Software
Scope Note:
The Video Editing Software class refers to the specific applications or programs used to perform the editing operations on the video produced from the 3D model rendering. This software provides tools and features necessary for video manipulation and enhancement, enabling users to create professional-quality videos.

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
The Project Video class refers to the final video product that contains the rendered 3D model, after undergoing editing processes. This video represents the completed work, showcasing the 3D model in a polished format, and is typically used for presentations, marketing, or documentation purposes.

Examples:
The final video output showcasing a 3D architectural design, ready for client delivery.
A promotional video that highlights the features of a virtual tour created from a 3D model.
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
The AR 3D Model class refers to a 3D model that has been modified and prepared for implementation in an Augmented Reality (AR) or Mixed Reality (MR) project. This model is designed to interact with real-world environments and enhance user experiences through digital overlays.

Examples:

A 3D reconstruction of a historical site intended for an AR application.
A virtual artifact designed to be viewed in a mixed reality setting.
Label: ExportedAR3DModel
---------------------------------------------------------------------------
F98 AR/MR Project Implementation
URI: https://photogrammetry.altervista.org/items/show/185 
SubClass of: 
D7 Digital Machine Event

Scope Note:
The AR/MR Project Implementation class refers to the process of integrating the AR 3D model (F97) into a specific Augmented Reality or Mixed Reality project. This includes the technical steps required to ensure the model functions properly within the AR/MR environment.

Examples:

Loading a 3D model into an AR application for mobile devices.
Integrating a virtual object into a mixed reality experience for educational purposes.
Label: Exporting_AR-MRProjectImplementation

---------------------------------------------------------------------------
F99 AR Software Modelling
URI: https://photogrammetry.altervista.org/items/show/186 
SubClass of: 
D14 Software

Scope Note:
The AR Software Modelling class refers to the software used in the Augmented Reality or Mixed Reality project where the AR 3D model (F97) has been loaded. This software facilitates the creation and deployment of interactive AR experiences.

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
The Survey Phase refers to a stage within the acquisition process, which can be divided into various moments such as acquisition, processing, and analysis. Each phase within the survey process addresses a specific task or set of tasks that contribute to the overall objective of collecting spatial, visual, or other relevant data about an object or environment. A Survey Phase may encompass the preparation of equipment, calibration, field operations, and initial data checks, ensuring that the collected data adheres to predefined technical standards. The phases may vary depending on the project’s design and procedural requirements, contributing to the systematic and reproducible execution of the survey.

Examples:
The Survey Phase involved an initial site walk-through and preparation, followed by the actual data acquisition using a terrestrial laser scanner.
Label: SurveyPhase

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
—-----------------------------------------------------------------------
F104: Registration (Fusion of Multiple Point Clouds or 3D Models)
URI: https://photogrammetry.altervista.org/items/show/190 
Subclass of:

F27 Densified Cloud Point

Scope Note:
The F104 Registration class refers to the process of aligning and merging multiple point clouds or 3D models into a single, coherent model. This class captures the concept of registration, a key step in photogrammetry and 3D reconstruction workflows where data collected from different viewpoints or sources is combined to create a comprehensive representation of an object or scene.
In this process, registration involves the precise alignment of overlapping regions of point clouds or 3D models, ensuring that they share a common coordinate system and that the surfaces match accurately. This can be done manually or, more commonly, through automated algorithms that minimize alignment errors by detecting corresponding points or features across the datasets.
Registration is an essential step, especially when working with large datasets or complex scenes that require the integration of multiple scans. This class describes the methodology and actions taken to perform the registration, including the matching of common features, alignment algorithms used, and optimization techniques to reduce errors.
F104 is a subclass of F27 Densified Cloud Point, as registration often begins with individual densified point clouds—highly detailed datasets representing surfaces—which are then combined into a unified model for further processing or analysis.

Examples:

The registration (F104) of two overlapping point clouds from different vantage points was performed to generate a complete 3D model of an ancient temple.
During the photogrammetric survey of a large site, registration (F104) was used to merge multiple 3D models captured from different sections, resulting in a unified representation of the site.
Automated registration (F104) was applied to fuse point clouds captured from aerial and ground-based photogrammetry, creating a comprehensive 3D model for analysis.

Label: ProcessedDensifiedPointCloudRegistration




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
—------------------------------------------------------------------------
Y24: happened on processing device
URI: https://photogrammetry.altervista.org/items/show/215 
Subproperty of: L12 happened on device
Domain: F3 Processing
Range: F10 Processing Device, F56  Mesh Reconstruction, F57  Texturing Mesh

Scope Note:
This property associates the processing phase (F3) with the processing device (F10) on which the processing occurred.

Example:
A processing phase F3 Processing happens on a F10 Processing Device, such as a high-performance server.

Label: happened_on_processing_device
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

Y63: has date of acquisition
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
Range: F29 Textured 3D Model

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
Domain: Editing Video
Range: 3D Model Video Rendering

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

Y80: is in GIS
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
Range: F84 3D Model Prospectus

Scope Note:
This property indicates that the CAD analysis (CAD Analysis) produced a 3D model prospectus (3D Model Prospectus) as its output.

Example:
  
Label: had_prospectus_output
—------------------------------------------------------------------------

Y85: had archaeometric input
URI: https://photogrammetry.altervista.org/items/show/274 
Subproperty of: L10 had input
Domain: Project Analysis
Range: Archaeometric 3D Model

Scope Note:
This property specifies that the project analysis (Project Analysis) used an archaeometric 3D model (Archaeometric 3D Model) as an input for detailed material or structural analysis.

Example:
  
Label: had_archaeometric_input
—------------------------------------------------------------------------

Y86: had data log analysis output
URI: https://photogrammetry.altervista.org/items/show/273 
Subproperty of: L11 had output
Domain: Project Analysis
Range: Data Log Analysis

Scope Note:
This property indicates that the project analysis phase (Project Analysis) resulted in a data log analysis (Data Log Analysis) as its output.

Example:
  
Label: had_data_log_analysis_output
—------------------------------------------------------------------------

Y87: had 3D model interactive as input
URI: https://photogrammetry.altervista.org/items/show/272 
Subproperty of: L10 had input
Domain: Interactive Project
Range: 3D Model for Interactive

Scope Note:
This property shows that the interactive project (Interactive Project) used a 3D model designed for interactive use (3D Model for Interactive) as its input.

Example:
  
Label: had_interactive_tridimensional_model_as_input
—------------------------------------------------------------------------

Y88: used interactive software
URI: https://photogrammetry.altervista.org/items/show/271 
Subproperty of: L23 used software
Domain: Interactive Project
Range: Interactive Software

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


