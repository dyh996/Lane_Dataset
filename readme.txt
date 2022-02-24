# HL20200113045424_0_IMU.bin
	IMU data file, incremental IMU data ，
	7 columns double [weeksec(s), gyrx(rad), gyry(rad), gyrz(rad), accx(m/s), accy(m/s), accz(m/s)]
	
# HL20200113045424_0_ODO.txt
	Odometer data file,
	3 columns  [weeksec(s), odoleft(m/s), odoright(m/s)]
	
# HL20200113045424_0_GNSS.txt
	GNSS positioning file, 
	7 columns  [weeksec(s), lat(deg), lon(deg), alt(m), latstd(m), lonstd(m), altstd(m)]
	
# LC_SM_TXT.nav
	The projected reference file
	11 columns [week, weeksec(s), lat(deg), lon(deg), alt(m), V_N(m/s), V_E(m/s), V_D(m/s), roll(deg), pitch(deg), heading(deg)]

# 05.bag(extract from rar package(camera_data.rar))
	Real-time photo file 
	topic name: /cam0/image_raw
	
# map.txt
	Lane map file
	5 columns [the three-direction coordinates (Gaussian projection) of the dotted line endpoint, the width of the left lane and the width of the right lane]
	
# Installation parameters
	antenna lever:  [-0.34, 0.0, 0.14](m) #  IN the coordinate system of the IMU, where the X-axis is pointing forweard, Y-axis is pointing right and Z-axis is pointing down. 
	odometer lever: [0.0, 0.0, 0.93](m)   #  same as above
	camera lever：  [0.08, -0.07, -0.01](m) #  same as above
	
# IMU parameters
	Device: ADIS16465
	arw: 0.2  #deg/sqrt(h)
	vrw: 0.2  #m/s/sqrt(h)
	std_gb: 20  #deg/h
	std_ab: 100  #mGal
	std_gs: 100  #PPM
	std_as: 100  #PPM
	
# ODO parameters
	std_os: 500  #PPM
	
# Camera parameters
	Device： 	 Mako G-131C 
	Color:   	 BayerBG8
	Resolution:  1278x1022
	Frame rate:  20HZ
	distortion_coeffs: [-0.0927, 0.0869, -9.5115e-05, 5.1090e-04]
	intrinsic matrix:   [790.8231, 0.,664.9502, 0., 791.4002, 520.0424, 0., 0., 1.]
	