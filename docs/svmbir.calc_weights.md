# ``svmbir.calc_weights``

**Signature:**

	svmbir.calc_weights( 
		sino, 
		weight_type="unweighted"
	) 

Computes the weights used in reconstruction. 

**Parameters:**

 * ``sino``: 3D numpy array of sinogram data organized with ``sino[slice,channel,view]``.

 * ``weight_type``: [Default="unweighted"] Type of noise model used for data. 

With this routine, the weights can be computed manually and passed to the ``recon`` routine. This is equivalent to only passing the ``weight_type`` parameter to the ``recon`` routine.
	
**Returns:**

 * ``weights``: Calculated values of ``weights`` parameter.

# What it does:

This function computes weights using the values of the ``weight_type`` parameters as shown below:

	If weight_type="unweighted"        => weights = numpy.ones_like(sino)
	If weight_type="transmission"      => weights = numpy.exp(-sino)
	If weight_type="transmission_root" => weights = numpy.exp(-sino/2)
	If weight_type="emmission"         => weights = 1/(sino + 0.1)

#Example Usage:
