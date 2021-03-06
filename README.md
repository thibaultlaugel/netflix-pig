# Using Map Reduce (Pig) for recommendations
This project is a following of the one that can be found in the repository: http://github.com/thibaultlaugel/netflix-privacy

The goal of this project is to use the Map Reduce technology to tackle the dimensionnality issue raised by our first attempt at solving the Netflix recommendations problem. We used PIG to compute our recommendations on a Microsoft Azure cluster.

Despite based on the same data, this project does not focus like the first one on ensuring privacy of the users, but rather on using all data available to find the best movie recommendations. Thus, the computation of the movie/user effects is simplified. Moreover, we also decided not to include the SVD decomposition to focus on the k-NN algorithm.

_________________________
Files description:

Main Files:
- Donnees_Massives.pdf: project report (French)
- compute_covar_matrix.pig: PIG script for computation of the movie-movie covariance matrix
- compute_effects.pig: PIG script for the computation of the movie and user effects
- compute_pred.pig: PIG script for the computation of the final rating predictions

Other:
- create_train_test.pig
