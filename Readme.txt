How To Run:


1. Keep em_data.txt and Em_algo.py in the same folder.
2. Run python Em_algo.py code in command prompt
    (I have used spyder IDE. Load the file and run the file)

4. K=3 number of clusters
    Mean values are randomly selected by: file[np.random.choice(n, self.k, False), :] (file reads data from em_data.txt file)
    Co-varience are initially selected as: sigmas = np.array([np.eye(p)] * self.k) 
	For varience 0: sigmas = np.array([[[ 7.67788792]] ,[[ 7.67788792]], [[ 7.67788792]]])  or to select random sigmas *= np.random.uniform(1, 10)
    Max iteraton : 80 epsilon: 0.01
5. Initialization strategy used: initial K Gaussian means by randomly selecting K initial data points, and selected the initial K random variances
