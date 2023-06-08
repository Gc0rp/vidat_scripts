# vidat_scripts


Polygon Points and Spatial Interpolation Parameters:

Instructions: 

Modify the last cell with the following parameters

x = (An integer containing the number of frames) # Number of frames

operation = ('-' or '+') '-' is for Monotonically decreasing and '+' is for Monotonically increasing

polygon_A = A numpy array of coordinates

polygon_B = A numpy array of coordinates

segments_A = A numpy array containing a 2D array showing the connecting between each segment 

segments_B = A numpy array containing a 2D array showing the connecting between each segment 



Example of a monontonically decreasing polygon:

x = 12 # Number of frames

operation = '-' # Monotonically decreasing

polygon_A = np.array([[5,0], [0,4], [6,5], [7,5], [7,0]])

polygon_B = np.array([[0,0],[1,0],[0,2]]) # Polygon B (Final state)

segments_A = np.array([[[5,0], [0,4]], [[0,4], [6,5]], [[6,5], [7,5]], [[7,5], [7,0]], [[7,0], [5,0]]])

segments_B = np.array([[[0,0], [0,2]], [[0,2], [1,0]], [[1,0], [0,0]]])
