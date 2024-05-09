# Quantum_VS_Classical_Clustering
A comparison between both Quantum and Classical clustering using K-Means Algorithm. this project shows the steps and differences between both with implementation from Scratch.

## Classical Clustering (KMeans algorithm):
**Steps**:
   - determine the number of clusters
   - randomly initialize the centroids
   - measure distances between data points and the centroids >> Fidelity
   - assign data points to the nearest centroid
   - update the position of the centroid according to the mean of each cluster

## Quantum Clustering for single feature :
**Steps**:
  - determine the number of clusters
  - randomly initialize the centroids
      - measure distances between data points and the centroids `Fidelity`
      - Initialize three separable states in the ground state. One is for the data point and the other two represent the centroid.
      - choose your encoding scheme
      - using a for loop you will pick a classical point to measure the distance between the centroids and this sample.
      - encode the data using the encoding scheme (rotational gates)
      - apply the selected rotational gates on the states
      - then calculate the fidelity between the two states (one state would represent the data point and the other would represent the centroid
  - assign data points to the nearest centroid
  - update the position of the centroid according to the mean of each cluster

## Data Representation and Encoding
Data points are represented as quantum states (qubits) in the computational basis. For one feature, each data point is encoded as a single qubit using an encoding scheme(rotational gates).

## Fidelity: 
Fidelity is a measure of the "closeness" of two quantum states and is the inner product between two states.

## Dependencies:
This project requires the installation of the following libraries:
- qiskit
- numpy
- pandas
- matplotlib
- sklearn
- scipy
  

