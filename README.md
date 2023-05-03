Download Link: https://assignmentchef.com/product/solved-cs2100-tutorial-7-combinational-circuits
<br>
D1. Design a circuit, without using any logic gate, that takes a 3-bit input <em>ABC</em> representing an unsigned integer <em>x</em>, and produces a 5-bit output <em>VWXYZ</em> which is equivalent to 4<em>x</em>+2. What are <em>V</em>, <em>W</em>, <em>X</em>, <em>Y</em> and <em>Z</em>?




D2. The following algorithm to convert binary to standard Gray code sequence is given in Digital Logic Design page 35:

<ol>

 <li>Retain the MSB.</li>

 <li>From left to right, add each adjacent pair of binary code bits to get the next Gray code bit, discarding the carry.</li>

</ol>




The following example shows the conversion of binary number (10110)<sub>2</sub> to its corresponding standard Gray code value, (11101)<sub>Gray</sub>.

<sup>                </sup>1 0 1 1 0 Binary                  <u>1</u> + <u>0</u> 1 1 0 Binary                   1 <u>0</u> + <u>1</u> 1 0 Binary

<sub>            </sub>↓                                                ↓                                               ↓

<strong>1 </strong>                    Gray               1  <strong>1 </strong>               Gray                1 1  <strong>1 </strong>              Gray




1 0 <u>1</u> + <u>1</u> 0 Binary                     1 0 1 <u>1</u> + <u>0</u> Binary

<sup>                              </sup>1  1  1    ↓<strong>0</strong> <strong> </strong>       Gray               1  1  1  0    <strong>1</strong>↓ <strong>    </strong>Gray




Given a half-adder as shown on the right where <em>X</em> and <em>Y</em> are its inputs and <em>C</em> (carry) and <em>S</em> (sum) its outputs,

implement a 5-bit binary to Gray code converter to <em>X    Y </em>convert the binary value <em>ABCDE</em> to its equivalent Gray  code <em>PQRST</em> by using the fewest number of half- <em>C    S </em>adders without any additional logic gates.




<h2>D3. [Past year’s question]</h2>

A combinational circuit takes in a 5-bit input <em>ABCDE</em> and generates a 2-bit value <em>PQ</em> such that <em>PQ</em> represents the <em>distance</em> between the two closest 1s in the input. The distance is defined to be the number of 0s between the two closest 1s.

For example, if <em>ABCDE</em> is 01011, then the distance between the two closest 1s (the two rightmost 1s) is zero, therefore, <em>PQ</em>=00. If <em>ABCDE</em> is 10010, then the distance between the two closest 1s is 2, therefore, <em>PQ</em>=10.

You may assume that the distance is always determinable from the given input. Therefore, inputs such as 00000 and 01000 will not be supplied to this circuit.

Draw the K-maps for <em>P</em> and <em>Q</em> and write the simplified SOP expressions for <em>P</em> and <em>Q</em>.

Using the simplified SOP expressions for <em>P</em> and <em>Q</em> to implement the circuit, what is the output if the circuit is fed with the input <em>ABCDE</em>=00100?







<strong>Tutorial questions </strong>

Note that for questions on logic design, you may assume that logical constants 0 and 1 are always available. However, complemented literals are <u>not available</u> unless otherwise stated.




<h2>1.  [Past-year’s question]</h2>

You are to design a circuit to implement a function <em>V</em>(<em>A</em>,<em>B</em>,<em>C</em>,<em>D</em>,<em>E</em>) that takes in input <em>ABCDE</em> and generates output 1 if <em>ABCDE</em> is a valid input for the circuit in question D3 above, or 0 if <em>ABCDE</em> is an invalid input. You are allowed to use only the following devices: full adder, 2-bit parallel adder, and 4-bit magnitude comparator. You should use the fewest number of these approved devices, and <u>no other devices or logic gates</u>. The block diagrams for these devices are shown below.













<h2>2.    [Past year’s exam question]</h2>

<ol start="2">

 <li>You want to construct a circuit that takes in a 4-bit unsigned binary number <em>ABCD</em> and outputs a 4-bit unsigned binary number <em>EFGH</em> where <em>EFGH</em> = (<em>ABCD</em> + 1) / 2. Note that the division is an integer division. For example, if<em> ABCD</em> = 0110 (or 6 in decimal), then <em>EFGH</em> = 0011 (or 3 in decimal). If <em>ABCD</em> = 1101 (or 13 in decimal), then <em>EFGH</em> = 0111 (or 7 in decimal).</li>

</ol>

Construct the above circuit using a single <strong>4-bit parallel adder</strong> and at most one logic gate with no restriction on its fan-in.

<ol start="9">

 <li>The following table shows the 4221 code and 8421 code (also known as BCD code) for the ten decimal digits 0 through 9.</li>

</ol>

<table width="274">

 <tbody>

  <tr>

   <td width="70"><strong>Digit </strong></td>

   <td width="102"><strong>4221 code </strong></td>

   <td width="102"><strong>8421 code </strong></td>

  </tr>

  <tr>

   <td width="70">0</td>

   <td width="102">0000</td>

   <td width="102">0000</td>

  </tr>

  <tr>

   <td width="70">1</td>

   <td width="102">0001</td>

   <td width="102">0001</td>

  </tr>

  <tr>

   <td width="70">2</td>

   <td width="102">0010</td>

   <td width="102">0010</td>

  </tr>

  <tr>

   <td width="70">3</td>

   <td width="102">0011</td>

   <td width="102">0011</td>

  </tr>

  <tr>

   <td width="70">4</td>

   <td width="102">0110</td>

   <td width="102">0100</td>

  </tr>

  <tr>

   <td width="70">5</td>

   <td width="102">1001</td>

   <td width="102">0101</td>

  </tr>

  <tr>

   <td width="70">6</td>

   <td width="102">1100</td>

   <td width="102">0110</td>

  </tr>

  <tr>

   <td width="70">7</td>

   <td width="102">1101</td>

   <td width="102">0111</td>

  </tr>

  <tr>

   <td width="70">8</td>

   <td width="102">1110</td>

   <td width="102">1000</td>

  </tr>

  <tr>

   <td width="70">9</td>

   <td width="102">1111</td>

   <td width="102">1001</td>

  </tr>

 </tbody>

</table>




You want to construct a 4221-to-8421 decimal code converter, which takes in a 4-bit 4221 decimal code <em>PQRS</em> and generates the corresponding 4-bit 8421 decimal code <em>WXYZ</em>.

Let’s call the circuit you created in part (a) above the A1H (Add-1-then-Half) device, represented by the block diagram below. Implement your 4221-to-8421 decimal code converter using this A1H device with the fewest number of additional logic gates.







<h2>3.    [Past year’s exam question]</h2>

The BCD code (also known as 8421 code) values for the ten decimal digits are given below:




<table width="549">

 <tbody>

  <tr>

   <td width="52">Digit:</td>

   <td width="50">0</td>

   <td width="50">1</td>

   <td width="50">2</td>

   <td width="50">3</td>

   <td width="50">4</td>

   <td width="50">5</td>

   <td width="50">6</td>

   <td width="50">7</td>

   <td width="50">8</td>

   <td width="49">9</td>

  </tr>

  <tr>

   <td width="52">Code:</td>

   <td width="50">0000</td>

   <td width="50">0001</td>

   <td width="50">0010</td>

   <td width="50">0011</td>

   <td width="50">0100</td>

   <td width="50">0101</td>

   <td width="50">0110</td>

   <td width="50">0111</td>

   <td width="50">1000</td>

   <td width="49">1001</td>

  </tr>

 </tbody>

</table>




For example, the decimal value 396 is represented as 0011 1001 0110 in BCD code.

Given two decimal digits <em>A</em> and <em>B</em>, represented by their BCD codes <em>A</em><sub>3</sub><em>A</em><sub>2</sub><em>A</em><sub>1</sub><em>A</em><sub>0</sub> and <em>B</em><sub>3</sub><em>B</em><sub>2</sub><em>B</em><sub>1</sub><em>B</em><sub>0</sub> respectively, implement a circuit <u>without using any logic gates</u> to calculate the BCD code of the 3-digit output of (51<em>A</em>) + (20(<em>B</em>%2)), where % is the modulo operator. Name the outputs <em>F</em><sub>11</sub><em>F</em><sub>10</sub><em>F</em><sub>9</sub><em>F</em><sub>8  </sub><em>F</em><sub>7</sub><em>F</em><sub>6</sub><em>F</em><sub>5</sub><em>F</em><sub>4  </sub><em>F</em><sub>3</sub><em>F</em><sub>2</sub><em>F</em><sub>1</sub><em>F</em><sub>0</sub>.

For example, if <em>A</em>=2 (or 0010 in BCD) and <em>B</em>=7 (or 0111 in BCD), then (51<em>A</em>) + (20(<em>B</em>%2)) = 122 or 0001 0010 0010 in BCD. Hence, the circuit is to produce the output 0001 0010 0010 for the inputs 0010 and 0111.

[<em>Hint:</em> Fill in the table below that computes 5<em>A</em>.]




<table width="506">

 <tbody>

  <tr>

   <td width="44"> </td>

   <td width="40"> </td>

   <td colspan="2" width="49"><em>A </em></td>

   <td width="45"> </td>

   <td colspan="8" rowspan="2" width="328">5<em>A</em></td>

  </tr>

  <tr>

   <td width="44"><em>A</em><sub>3</sub></td>

   <td width="40"><em>A</em><sub>2</sub></td>

   <td width="5"> </td>

   <td width="44"><em>A</em><sub>1</sub></td>

   <td width="45"><em>A</em><sub>0</sub></td>

  </tr>

  <tr>

   <td width="44">0</td>

   <td width="40">0</td>

   <td width="5"> </td>

   <td width="44">0</td>

   <td width="45">0</td>

   <td width="40"> </td>

   <td width="40"> </td>

   <td width="40"> </td>

   <td width="40"> </td>

   <td width="42"> </td>

   <td width="42"> </td>

   <td width="42"> </td>

   <td width="42"> </td>

  </tr>

  <tr>

   <td width="44">0</td>

   <td width="40">0</td>

   <td width="5"> </td>

   <td width="44">0</td>

   <td width="45">1</td>

   <td width="40"> </td>

   <td width="40"> </td>

   <td width="40"> </td>

   <td width="40"> </td>

   <td width="42"> </td>

   <td width="42"> </td>

   <td width="42"> </td>

   <td width="42"> </td>

  </tr>

  <tr>

   <td width="44">0</td>

   <td width="40">0</td>

   <td width="5"> </td>

   <td width="44">1</td>

   <td width="45">0</td>

   <td width="40"> </td>

   <td width="40"> </td>

   <td width="40"> </td>

   <td width="40"> </td>

   <td width="42"> </td>

   <td width="42"> </td>

   <td width="42"> </td>

   <td width="42"> </td>

  </tr>

  <tr>

   <td width="44">0</td>

   <td width="40">0</td>

   <td width="5"> </td>

   <td width="44">1</td>

   <td width="45">1</td>

   <td width="40"> </td>

   <td width="40"> </td>

   <td width="40"> </td>

   <td width="40"> </td>

   <td width="42"> </td>

   <td width="42"> </td>

   <td width="42"> </td>

   <td width="42"> </td>

  </tr>

  <tr>

   <td width="44">0</td>

   <td width="40">1</td>

   <td width="5"> </td>

   <td width="44">0</td>

   <td width="45">0</td>

   <td width="40"> </td>

   <td width="40"> </td>

   <td width="40"> </td>

   <td width="40"> </td>

   <td width="42"> </td>

   <td width="42"> </td>

   <td width="42"> </td>

   <td width="42"> </td>

  </tr>

  <tr>

   <td width="44">0</td>

   <td width="40">1</td>

   <td width="5"> </td>

   <td width="44">0</td>

   <td width="45">1</td>

   <td width="40"> </td>

   <td width="40"> </td>

   <td width="40"> </td>

   <td width="40"> </td>

   <td width="42"> </td>

   <td width="42"> </td>

   <td width="42"> </td>

   <td width="42"> </td>

  </tr>

  <tr>

   <td width="44">0</td>

   <td width="40">1</td>

   <td width="5"> </td>

   <td width="44">1</td>

   <td width="45">0</td>

   <td width="40"> </td>

   <td width="40"> </td>

   <td width="40"> </td>

   <td width="40"> </td>

   <td width="42"> </td>

   <td width="42"> </td>

   <td width="42"> </td>

   <td width="42"> </td>

  </tr>

  <tr>

   <td width="44">0</td>

   <td width="40">1</td>

   <td width="5"> </td>

   <td width="44">1</td>

   <td width="45">1</td>

   <td width="40"> </td>

   <td width="40"> </td>

   <td width="40"> </td>

   <td width="40"> </td>

   <td width="42"> </td>

   <td width="42"> </td>

   <td width="42"> </td>

   <td width="42"> </td>

  </tr>

  <tr>

   <td width="44">1</td>

   <td width="40">0</td>

   <td width="5"> </td>

   <td width="44">0</td>

   <td width="45">0</td>

   <td width="40"> </td>

   <td width="40"> </td>

   <td width="40"> </td>

   <td width="40"> </td>

   <td width="42"> </td>

   <td width="42"> </td>

   <td width="42"> </td>

   <td width="42"> </td>

  </tr>

  <tr>

   <td width="44">1</td>

   <td width="40">0</td>

   <td width="5"> </td>

   <td width="44">0</td>

   <td width="45">1</td>

   <td width="40"> </td>

   <td width="40"> </td>

   <td width="40"> </td>

   <td width="40"> </td>

   <td width="42"> </td>

   <td width="42"> </td>

   <td width="42"> </td>

   <td width="42"> </td>

  </tr>

 </tbody>

</table>




Complete the circuit below:



















<sub>                                       </sub><em>F</em><sub>11</sub>   <em>F</em><sub>10</sub>   <em>F</em><sub>9</sub>    <em>F</em><sub>8</sub><em>    F</em><sub>7</sub>    <em>F</em><sub>6</sub>    <em>F</em><sub>5</sub>    <em>F</em><sub>4</sub><em>    F</em><sub>3</sub>    <em>F</em><sub>2</sub>    <em>F</em><sub>1</sub>    <em>F</em><sub>0</sub>




<ol start="4">

 <li>Given a 4-bit magnitude comparator as shown on the right, implement the following 4-variable Boolean functions using only this single magnitude comparator with <u>no</u> other logic gates. (Note that there could be multiple answers.) (a) <em>F</em>(<em>A</em>,<em>B</em>,<em>C</em>,<em>D</em>) = <em>m</em>(12 – 15).</li>

</ol>

<ul>

 <li><em>G</em>(<em>A</em>,<em>B</em>,<em>C</em>,<em>D</em>) = <em>m</em>(0, 6, 9, 15).</li>

 <li><em>H</em>(<em>A</em>,<em>B</em>,<em>C</em>,<em>D</em>) = <em>m</em>(0, 1, 6, 7, 8, 9, 14, 15).</li>

 <li><em>Z</em>(<em>A</em>,<em>B</em>,<em>C</em>,<em>D</em>) = <em>m</em>(1, 3, 5, 7, 9, 11, 13).</li>

</ul>