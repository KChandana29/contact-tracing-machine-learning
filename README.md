# Contact Tracing Application
This Python script is a contact tracing application that uses the DBSCAN (Density-Based Spatial Clustering of Applications with Noise) algorithm and K-means clustering to identify potential contacts who might have been infected by a person based on their geospatial data. 

# How to Use
Upon running the script, you'll see a menu with two options:

 Find who a person might have infected: This option allows you to enter the name of a person, and the application will identify and display individuals who might have been infected by that person based on a predefined distance threshold (1 km by default). The application uses geospatial data and calculates distances to determine potential contacts.

Exit: This option allows you to exit the application.

# Notes on Clustering
The application uses two clustering algorithms:

DBSCAN: This algorithm identifies clusters of geospatial points. The clustering parameters (epsilon and min_samples) can be adjusted to affect the cluster formation. The silhouette score is calculated to evaluate the quality of the DBSCAN clustering.

K-means: This algorithm is used to cluster geospatial points into a predefined number of clusters. The silhouette score is also calculated to evaluate the quality of the K-means clustering.

# Additional Information
The application displays geospatial data as a scatter plot before clustering.
After clustering, the application displays the results with different cluster colors.
The DBSCAN clustering result may include a single cluster, which indicates noise. Adjust the DBSCAN parameters accordingly.
