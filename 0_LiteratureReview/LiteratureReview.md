# Literature Review

Approaches or solutions that have been tried before on similar projects.

**Summary of Each Work**:

- **Source 1**: Benchmarking and Automating the Image Recognition Capability of an In Situ Plankton Imaging System

  - **[https://www.frontiersin.org/articles/10.3389/fmars.2022.869088/full]()**
  - **Objective**: Assess and improve the image recognition capability of the in situ Scripps Plankton Camera (SPC) system for plankton identification.
  - **Methods**: Employed Convolutional Neural Networks (CNNs), specifically the ResNet-18 architecture, for image classification. The study compared automated counts from SPC with manual counts from lab-based methods.
  - **Outcomes**: Achieved an average accuracy of 92% in CNN-based plankton identification and demonstrated a good correlation between automated and manual counting methods.
  - **Relation to the Project**: Fine Tuning from ResNet-18 can be a valid approach for our task.

- **Source 2**: A Convolutional Neural Network to Classify Phytoplankton Images Along the West Antarctic Peninsula

  - **[https://www.ingentaconnect.com/contentone/mts/mtsj/2022/00000056/00000005/art00001]()**
  - **Objective**: Develop a Convolutional Neural Network (CNN) to classify phytoplankton images collected with an Imaging FlowCytobot for the Palmer Antarctica Long-Term Ecological Research project.
  - **Methods**: A small CNN (~2 million parameters) was created and trained using a subset of manually identified images.
  - **Outcomes**: The CNN achieved high accuracy on a balanced dataset but faced challenges in natural environments due to class imbalances and morphological similarities among phytoplankton.
  - **Relation to the Project**: Training our own CNN might be a good approach as well, as we have the data already labeled and available. We might also be able to achieve really good results by breaking down the problem into a system, that classifies the phytoplankton 4 at a time and then continues to feed this information into the next NN.

- **Source 3**: Improving Plankton Image Classification Using Context Metadata

  - **[https://aslopubs.onlinelibrary.wiley.com/doi/epdf/10.1002/lom3.10324]()**
  - **Objective**: Enhance plankton image classification by incorporating context metadata.
  - **Methods**: Utilized a Convolutional Neural Network (CNN) combined with context metadata such as date, time, depth, and location.
  - **Outcomes**: Demonstrated improved classification accuracy, highlighting the significance of context metadata alongside traditional image features in plankton image classification.
  - **Relation to the Project**: The metadata in our case is likely limited, however we can still benefit from adding more "variables" to the classes, as an intention to improve the classification result.
