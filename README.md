# Cadence NatureDSP Library for ConnX B20 DSP cores

<p>This NatureDSP Library for ConnX B20 DSP contains various optimized general purpose signal processing routines.</p>
 <h1> Version: v3.2.0 </h1>
<p> This patch release contains following changes compared to the previous release v3.0.0:</p>
  <h3> Changes:</h3>
        <p>
        <ol>
        <li>Replaced first step of Newton-Raphson based single precision floating point reciprocal
  operation & other sequence of instructions with a direct RECIP proto.</li>
        <li>Updated the code to use Quadratic Lagrange Interpolation(QLI) based single precision
  floating point reciprocal operation where ever applicable.</li>
         <li>Newly added support over various precisions and categories are listed below. </li>
         <p>
          <ol>
         <li>Double Precision</li>
           <ol>
     <li>math, complex math and Vector(scale,add and norm) APIs. </li>
     <li>Streaming and block matrix operations cmatmul, cmatvmul, rcmatul, rcmatvmul, cmatherm, cmattrans,
	   matmult, vmatmul, cmatmult, cvmatmul, cmatmac, matmac, cmatmact, matmact,  matscale, cmatscale.</li>
    <li>Streaming/block conversion operations(cinterleave, cdeinterleave, cbs, csb).</li>
	<li>Complex APIs in Direct matrix inversion, Gauss Jordan inversion, LU & determinant, Cholesky and QR.</li>
     <li>polynomial fitting, tap based interpolation and Polynomial roots.</li>
	<li>real and complex Cholesky pseudo inversion and QR inversion.</li>
            </ol>
 <li>Single Precision</li>
     <ol>      
    <li>real & complex fft (N = 65536, 131072, 262144).</li>
	<li>cmatmulmxnxp, math (error function) and Vector( add ,scale).</li>
	<li>real and complex Cholesky pseudo inversion and QR inversion.</li>
	<li>Streaming and block matrix operations matmult, vmatmul, cmatmult, cvmatmul, cmatmac, matmac, cmatmact, matmact,  matscale, cmatscale.</li>
       </ol>
<li>Half precision </li>
           <ol>
    <li>cmatmulmxnxp, math (error function) and Vector( add ,scale).</li>
	<li>Streaming and block matrix operations matmult, vmatmul, cmatmult, cvmatmul, cmatmac, matmac, cmatmact, matmact,  matscale, cmatscale.</li>
            </ol>
 <li>32b fixed point</li>
            <ol>
    <li>Streaming and block matrix operations vmatmul, cvmatmul, cmatmac, matmac, matscale, cmatscale and Vector( add ,scale).</li>
             </ol>
 <li>16b fixed point</li>
           <ol>
    <li>Vector(add, scale) and Math (int2double, double2int)</li>
	   <li>Streaming and block matrix operations vmatmul, cvmatmul, cmatmac, matmac, matscale, cmatscale.</li>
          </ol>
        </li>
          </ol>
         </p> 
        </ol>
        </p>
        
 <h3>Details:</h3>
       <p>
       <ol>
      <li>This version of library has been tested with RI-2023.11 Xtensa tools.</li>
      </ol>
      </p>
<h3> Known issues:</h3>
     <p>
     <ol>
    <li> None</li>
     </ol>
     </p>

<h1> Version: v3.0.0 </h1>
 <h3> Details:</h3>
       <p>
       <ol>
      <li>This version of library has been optimized and tested with RI-2021.7 Xtensa tools.</li>
      </ol>
      </p>
<h3> Known issues:</h3>
     <p>
     <ol>
    <li> None</li>
     </ol>
     </p>



<h1>To use the library </h1>
<p>
<ol>
<li>Download the library & demo xws from the repository and import them into Xtensa Xplorer environment.</li>
<li>Upon importing, two directories i.e. b20_library & b20_demo  will be available in the Project Xplorer pane.</li>
<li>Refer to Chapter-3 of "NatureDSP_Baseband_B10_B20_Library_Reference.pdf" document present inside the b20_library/doc directory for details on build and run.</li>
<li>Detailed Release notes can be found at b20_library/doc directory.</li>
</ol>
</p>
