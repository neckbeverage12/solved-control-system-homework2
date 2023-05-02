Download Link: https://assignmentchef.com/product/solved-control-system-homework2
<br>
<ol>

 <li>Simulate spring-mass-damper system of unforced response with damping ratio equal to 0.3, 0.6, and 1 (see Fig. 2.46)</li>

</ol>

0.150.100.050

<ul>

 <li>05</li>

 <li>10</li>

 <li>15</li>

</ul>

<strong>FIGURE 2.46</strong>

Spring-mass-                            –<sub>0.20  </sub>

damper unforced                        0          1        2        3        4        5        6        7        <strong>8</strong>

response.                                                                               Time (s)

<ol start="2">

 <li>Simulate Example 2.19</li>

</ol>

<em>-_-;AAMPLE 2.</em><em> i</em><strong>            </strong><strong>Multiloop reduction</strong>

<strong>A rnultiloop </strong>feedback system <strong>is shown in Figure </strong>2.26. Our objective is to <strong>compute </strong><strong>the closed-loop transfer function, T(s), with</strong>

<strong><u>1                                      1 </u></strong>

G4(S)

<sup> 3(s) = </sup>S<sup>2______ </sup>+ <strong>4s + 4                        </strong>= <strong><em>s</em></strong>

<strong><u>s + 1 </u></strong>

<strong><em>Fl<sub>i</sub>(s) </em></strong><strong>=                        H<sub>2</sub>(s) = 2, and </strong><strong><em>//<sub>3</sub>(s) </em></strong><strong>= 1.</strong>

<strong>s +</strong>

<strong>For this example, a five-step procedure is followed:</strong>

<strong>Ul</strong><strong> Step 1. Input the system transfer functions,</strong>

<ul>

 <li><strong>Step 2. Move </strong><strong><em>H</em></strong><strong><em><sub>2</sub></em></strong><strong><em>(s) </em></strong><strong>behind G4(s)-</strong></li>

 <li><strong>Step 3. Eliminate the </strong>G((S) G4 <em>(S) (S) </em></li>

</ul>

<strong>F</strong><strong> Step 4. Eliminate the loop containing 11<sub>2</sub>(s).</strong>

<ul>

 <li><strong>Step 5. Eliminate the remaining loop and calculate T(s).</strong></li>

</ul>




The five steps are utilized in Figure 2.64, and the corresponding block diagram re­duction is shown in Figure 2.27. The result of executing the commands is

<em>s<sup>5</sup> + 4s<sup>4</sup> + 6s<sup>3</sup> + 6s<sup>2</sup> + 5s + </em><strong>2</strong>

sys = ____________________________________________________

123<sup>6</sup> + 205s<sup>5</sup> + 1066s<sup>4</sup> + 2517s<sup>3</sup> + 31.283<sup>2</sup> + 2196s + 712<sup>.</sup>

We must be careful in calling this the closed-loop transfer function. The transfer function is defined as the input—output relationship after pole—zero cancellations. If we compute the poles and zeros of <em>T(s), </em>we find that the numerator and denom­inator polynomials have <em>(s + </em>1) as a common factor. This must be canceled before we can claim we have the closed-loop transfer function. To assist us in the pole—zero cancellation, we will use the minreal <strong>function. The minreal function, </strong>shown in Figure 2.65, removes common pole—zero factors of a transfer function. The final step in the block reduction process is to cancel out the common factors, as shown in Figure 2.66. After the application of the minreal function, we find that the order of the denominator polynomial has been reduced from six to five, implying one pole—zero cancellation. ■

<em><u>H2(s)</u></em> G<sub>4</sub>(s)







<table>

 <tbody>

  <tr>

   <td width="156">

    <table width="100%">

     <tbody>

      <tr>

       <td>

        <table>

         <tbody>

          <tr>

           <td rowspan="2" width="28">(;<sub>1</sub>(s)</td>

           <td rowspan="2" width="70"></td>

           <td rowspan="2" width="26">020</td>

           <td width="27"> </td>

          </tr>

          <tr>

           <td width="27"> </td>

          </tr>

         </tbody>

        </table> </td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>

<table>

 <tbody>

  <tr>

   <td width="0"></td>

   <td width="2"></td>

   <td width="35"></td>

   <td width="30"></td>

   <td width="68"></td>

   <td width="21"></td>

   <td width="9"></td>

   <td width="22"></td>

   <td width="8"></td>

   <td width="189"></td>

  </tr>

  <tr>

   <td></td>

   <td colspan="2"></td>

   <td rowspan="7"></td>

  </tr>

  <tr>

   <td></td>

   <td colspan="2"></td>

   <td></td>

   <td colspan="2" rowspan="2"></td>

  </tr>

  <tr>

   <td></td>

   <td colspan="2"></td>

   <td></td>

   <td colspan="2"></td>

   <td rowspan="6"></td>

  </tr>

  <tr>

   <td></td>

  </tr>

  <tr>

   <td></td>

   <td rowspan="5"></td>

  </tr>

  <tr>

   <td></td>

   <td></td>

   <td></td>

   <td colspan="2"></td>

  </tr>

  <tr>

   <td></td>

  </tr>

  <tr>

   <td></td>

  </tr>

  <tr>

   <td></td>

   <td colspan="4"></td>

   <td colspan="2" rowspan="2"></td>

  </tr>

  <tr>

   <td></td>

  </tr>

 </tbody>

</table>

<table>

 <tbody>

  <tr>

   <td width="161">

    <table width="100%">

     <tbody>

      <tr>

       <td></td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>

<table>

 <tbody>

  <tr>

   <td width="83">

    <table width="100%">

     <tbody>

      <tr>

       <td>GO)</td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>




H<sub>3</sub>(s) rt____

(a)

______  62(s)

_____  H<sub>3</sub>(s)

( b




<strong><em>s</em></strong><strong> —O.                  GI</strong><strong><em>(s)</em></strong>

<strong>1 —          lei4(s )il </strong><strong><em>(s) </em></strong><strong>+ 62(.003(s)H2(s)</strong><strong><u> IT</u></strong>

P

<u>I </u>— 6<sub>3</sub>(s)G<sub>4</sub>C.011<sub>1</sub>(.0+ <em>Gi(s)G </em>.(N)14(N) + <em>G <sub>i</sub>(s). </em><em><sub>2</sub></em><em>0 ),G <sub>3</sub>006             </em><strong><em><sub>k</sub></em></strong><strong><em>(s</em></strong>

<strong><em><u>G </u></em></strong><u>i(N)G 2(.0G 3( .0G 4i.-F) </u>

<u>G2(S)G3(5)G4(5) </u>

<table>

 <tbody>

  <tr>

   <td width="112"></td>

  </tr>

  <tr>

   <td></td>

   <td></td>

  </tr>

 </tbody>

</table>




<table>

 <tbody>

  <tr>

   <td width="325">(c</td>

   <td width="310">(d)</td>

  </tr>

 </tbody>

</table>




<strong>FIGURE 2.26 </strong>Block diagram reduction of the system of Figure 2.25_




<strong>FIGURE </strong><strong>2.27 Signal-flow </strong>graph of the DC motor.

<strong>FIGURE 2.64</strong>

block

reduction.

<strong>FIGURE 2.65 </strong>The <strong>minreal </strong>function.

<strong>FIGURE 2.66</strong>

Application of the <strong>minreal </strong>function.




<ol start="3">

 <li>Simulate<strong> Example 2.20</strong></li>

</ol>

<em>EXAMPLE 2.20</em><strong> Electric traction motor control</strong>

Finally, let us reconsider the electric traction motor system from Example 2.13. The block diagram is shown in Figure 2.43(c). The objective is to compute the closed-loop transfer function and investigate the response of co(s) to a commanded w<sub>d</sub>(s). The first step, as shown in Figure 2.67, is to compute the closed-loop transfer func­tion co(s)/t_o<sub>d</sub>(s) = <em>T(s). </em>The closed-loop characteristic equation is second order with cia<sub>ii</sub> = 52 and = 0.012. Since the damping is low, we expect the response to be highly oscillatory. We can investigate the response <em>w(t) </em>to a reference input, <em>co<sub>d</sub>(t), </em>by utilizing the step function. The step function, shown in Figure 2.68, calculates the unit step response of a linear system. The step function is very important, since control system performance specifications are often given in terms of the unit step response.

If the only objective is to plot the output, <em>At), we </em>can use the step function without left-hand arguments and obtain the plot automatically with axis labels. If we need <em>y(t) </em>for any purpose other than plotting, we must use the <strong>step </strong>function with left-hand arguments, followed by the plot function to plot <em>y(t). </em>We define <em>t </em>as a row vector containing the times at which we wish the value of the output variable <em>y(I). </em>We can also select <em>t</em>

_ = _ <em>t</em>

<sub>final</sub>, which results in a step response from 1 = to <em>t </em>= t111 <sub>1</sub> and the number of intermediate points are selected automatically.

<em>EXAMPLE 2.13</em><strong> Electric traction motor control</strong>

The electric motor drive is shown in block diagram form in Figure 2.43(a), incor­porating the necessary control. The goal of the design is to obtain a system model and the closed-loop transfer function of the system, <em>w(s)/co<sub>d</sub>(s), </em>select appropriate resistors <strong><em>11, R2, R3, </em></strong>and <strong><em>R4, </em></strong>and then predict the system response.

The first step is to describe the transfer function of each block. We propose the use of a tachometer to generate a voltage proportional to velocity and to con­nect that voltage, v,, to one input of a difference amplifier, as shown in Figure 2.430). The power amplifier is nonlinear and can be approximately represented by v<sub>2</sub> (t) = 2e<sup>3</sup>v<sub>1</sub>(t) = g(2,<sub>1</sub>), an exponential function with a normal operating point, vto = 1.5 V. We then obtain a linear model

<table>

 <tbody>

  <tr>

   <td rowspan="2" width="153">40)<sub>2</sub>(0 =</td>

   <td colspan="2" width="45"><em><u>d(n) </u></em></td>

   <td rowspan="2" width="342"><strong>❑v<sub>i</sub>(t) = 6e<sup>3</sup>vt)Av<sub>1</sub>(t) = </strong>540 <strong>Av<sub>i</sub>(t).              </strong>(2.120)</td>

  </tr>

  <tr>

   <td width="42"> </td>

   <td width="3"> </td>

  </tr>

  <tr>

   <td width="153"> </td>

   <td width="42"> </td>

   <td width="3"> </td>

   <td width="342"> </td>

  </tr>

 </tbody>

</table>




Taking the Laplace transform, yields

V<sub>2</sub>(s) = 540AVi(s).




<table>

 <tbody>

  <tr>

   <td width="332"></td>

  </tr>

  <tr>

   <td></td>

   <td></td>

  </tr>

 </tbody>

</table>




<table>

 <tbody>

  <tr>

   <td rowspan="6" width="334"><strong>H</strong><strong>‘                                                     Power</strong><strong>amplifier</strong><strong>                       1 </strong>Sonsor _____</td>

   <td width="3"> </td>

   <td rowspan="3" width="55"><strong>A </strong><strong>rrnatu </strong>re-cOnliCoilCdMAGI’</td>

   <td width="48"> </td>

   <td width="1"> </td>

   <td width="50"> </td>

  </tr>

  <tr>

   <td width="3"> </td>

   <td width="48"> </td>

   <td width="1"> </td>

   <td width="50"> </td>

  </tr>

  <tr>

   <td width="3"> </td>

   <td width="48"> </td>

   <td width="1"> </td>

   <td width="50"> </td>

  </tr>

  <tr>

   <td width="3"> </td>

   <td width="55"> </td>

   <td width="48"> </td>

   <td width="1"> </td>

   <td width="50"> </td>

  </tr>

  <tr>

   <td width="3"> </td>

   <td width="55"> </td>

   <td width="48"> </td>

   <td width="1"> </td>

   <td width="50"> </td>

  </tr>

  <tr>

   <td width="3"> </td>

   <td width="55"> </td>

   <td width="48"> </td>

   <td width="1"> </td>

   <td width="50"> </td>

  </tr>

 </tbody>

</table>







<table>

 <tbody>

  <tr>

   <td width="546">

    <table width="100%">

     <tbody>

      <tr>

       <td> </td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>

<table>

 <tbody>

  <tr>

   <td width="464">

    <table width="100%">

     <tbody>

      <tr>

       <td></td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>

<table>

 <tbody>

  <tr>

   <td width="47">

    <table width="100%">

     <tbody>

      <tr>

       <td><strong>v</strong><strong><sub>2</sub></strong><strong>= 2diri </strong><strong>v</strong><strong><sub>io</sub></strong><strong>= 1.5</strong></td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>




<strong>FIGURE 243 </strong>Speed control of an electric <strong>traction </strong><strong>motor.</strong>




<strong>FIGUR E </strong><strong>2.67</strong><strong>Electric traction </strong><strong>motor block reduction.</strong>




<strong>Siep</strong><strong> _</strong><strong><sub>1</sub></strong><strong>1 </strong><strong>System </strong><strong>H</strong><strong><sub> Output</sub></strong>

<strong>input</strong><em>               </em><em>G(s)</em>

<strong>{</strong>