# home

The objective of this work is to tune the model predictive controller (MPC) to behave as a linear PI controller when constraints are inactive and act as a conventional MPC when constraints are active. A nonlinear optimization technique for MPC cost function minimization is proposed by solving linear matrix inequality (LMI) technique. We solve three different lemmas proposed by Cairano et. al. by using two methods:
i.	Solve-based and
ii.	Problem based. 
Resultant MPC gains are compared with the favorite feedback controller (PI) gains to understand the efficacy of the proposed lemmas. It was found out that all the lemmas were able to produce MPC gains quite close to the PI gains with an error less than 1%.   
This is unique for its ability to track linear feedback controller gains, especially in scenarios where system constraints are inactive. The optimized MPC was successfully integrated with a point absorber WEC model and was shown to handle various constraints. By incorporating linear controller characteristics within MPC frameworks, we achieve the benefits of both PI and MPC, ensuring maximum power absorption and constraint handling.
We investigate a WEC device model named WaveBot developed at Sandia National Laboratories to test the proposed MPC optimization technique. It is a point absorber designed to move in heave, surge, and pitch directions, but for simplicity, can be physically constrained to only heave. For the purpose of this example, we will focus solely on the heave mode of the WaveBot. The model-scale heaving point absorber was intended to replicate 1/17th of the size of a full-scale WEC. A CAD diagram of the WEC device and its physical characteristics are provided in Fig. 1.
<img width="290" alt="image" src="https://github.com/tashifat/home/assets/116129150/58696093-5e8e-4d11-a12c-2072e5de7931">


References
[1] H. Cho, G. Bacelli, and R. G. Coe, “Model Predictive Control Tuning by Inverse Matching for a Wave Energy Converter,” Energies, vol. 12, no. 21, Art. no. 21, Jan. 2019, doi: 10.3390/en12214158.
[2] S. Di Cairano and A. Bemporad, “Model Predictive Control Tuning by Controller Matching,” IEEE Transactions on Automatic Control, vol. 55, no. 1, pp. 185–190, Jan. 2010, doi: 10.1109/TAC.2009.2033838.
