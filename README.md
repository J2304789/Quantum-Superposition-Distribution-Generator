# Quantum Superposition Distribution Generator

### Developed by:

 - Muhammad Jawwad Javeed Iqbal [[Linkedin](https://linkedin.com/in/jawwad-javeed/)]


## 📚 Table of Contents

* [Project Purpose](#-project-purpose)
* [About](#-about)
* [Required Environment Installations](#-required-environment-installations)
* [File Navigation](#-file-navigation)
  * [Juypter Notebook Files](#juypter-notebook-files)
  * [Python Files](#python-files)
  * [Excel Files](#excel-files)
    * [Juypter Notebook](#juypter-notebook)
    * [Python](#python)
* [Notes](#-notes)
  * [Juypter Notebook](#juypter-notebook-1)
  * [Python](#python-1) 
  * [Excel](#excel)

## 📘 Project Purpose

The ability to specify Quantum Superposition Distributions (P(|0>) and P(|1>)) of a Qubit is effective for representing multiple complex states, an important attribute of Quantum computing that allows it to perform certain calculations more efficiently than a classical computer.

Currently however, it is difficult to specify a given probability distribution; for example, if the set distribution of P(|0>) and P(|1>) is selected to be 74%-26%,it would require trial and error in order to achieve the specific controlled rotation that would result in this Quantum Superposition Distribution(A demonstration of why simply entering a controlled rotation of a given percentage about a non-eigenstate axis would not work is available at [`Juypter_Notebook_Quantum_Superposition_Distribution_Generator_Demo.ipynb`](https://github.com/J2304789/Quantum-Superposition-Distribution-Generator/blob/main/Juypter_Notebook_Quantum_Superposition_Distribution_Generator/Juypter_Notebook_Quantum_Superposition_Distribution_Generator_Demo.ipynb))

This project aims to resolve this problem by using different Polynomial equations in order to predict the controlled rotations required for the specified Quantum Superposition Distribution.

## 📄 About

Qiskit Program that can generate a specified Quantum Superposition distribution (P(|0>) and P(|1>)) by utilizing Polynomial equations.

For this project it is recommended to use one of IBM's Quantum computers instead of a simulator in order to generate truly random numbers, however for testing purposes the [QASM Simulator](https://qiskit.org/documentation/stubs/qiskit.providers.aer.QasmSimulator.html#qasmsimulator) is the most accurate and similar to a real-life Quantum Simulator and is used as a proof of concept.


## 💻 Required Environment Installations

```
$ pip install Qiskit

``` 

## 🗃 File Navigation
- ### Juypter Notebook Files

  - [`Juypter_Notebook_Quantum_Superposition_Distribution_Generator_Demo.ipynb`](https://github.com/J2304789/Quantum-Superposition-Distribution-Generator/blob/main/Juypter_Notebook_Quantum_Superposition_Distribution_Generator/Juypter_Notebook_Quantum_Superposition_Distribution_Generator_Demo.ipynb) is a demonstration on why a given percentage controlled rotation about the y axis would result in significant errors for values that are not located on any of the bases |0>,|+>,or |1> 
  
  - [`Juypter_Notebook_Quantum_Superposition_Distribution_Generator_Polynomial.ipynb`](https://github.com/J2304789/Quantum-Superposition-Distribution-Generator/blob/main/Juypter_Notebook_Quantum_Superposition_Distribution_Generator/Juypter_Notebook_Quantum_Superposition_Distribution_Generator_Polynomial.ipynb) utilizes a polynomial function in order to scale the controlled rotations by a given percentage. However, because the values are predicted by a polynomial equation, they are highly inaccurate and are therefore left as a proof of concept (+/-95% error rate on both very low and very high numbers; average +/-35% error rate) and not recommended for any project utilization.
 
  - [`Juypter_Notebook_Quantum_Superposition_Distribution_Generator_Cubic.ipynb`](https://github.com/J2304789/Quantum-Superposition-Distribution-Generator/blob/main/Juypter_Notebook_Quantum_Superposition_Distribution_Generator/Juypter_Notebook_Quantum_Superposition_Distribution_Generator_Cubic.ipynb) utilizes a Cubic function in order to scale the controlled rotations by a given percentage. However, because the values are predicted by a Cubic equation, they are highly inaccurate and are therefore left as a proof of concept (+/-80% error rate on both very low and very high numbers; average +/-30% error rate) and not recommended for any project utilization.

  
  - [`Juypter_Notebook_Quantum_Superposition_Distribution_Generator_Quadratic.ipynb`](https://github.com/J2304789/Quantum-Superposition-Distribution-Generator/blob/main/Juypter_Notebook_Quantum_Superposition_Distribution_Generator/Juypter_Notebook_Quantum_Superposition_Distribution_Generator_Quadratic.ipynb) utilizes a Quadratic function in order to scale the controlled rotations by a given percentage. However, because the values are predicted by a Quadratic equation, they are highly inaccurate and are therefore left as a proof of concept (+/-80% error rate on both very low and very high numbers; average +/-20% error rate) and not recommended for any project utilization
  - [`Juypter_Notebook_Quantum_Superposition_Distribution_Generator_Quintic.ipynb`](https://github.com/J2304789/Quantum-Superposition-Distribution-Generator/blob/main/Juypter_Notebook_Quantum_Superposition_Distribution_Generator/Juypter_Notebook_Quantum_Superposition_Distribution_Generator_Quintic.ipynb) utilizes a Quintic function in order to scale the controlled rotations by a given percentage (+/-2% error rate on both very low and very high numbers; average +/-.5% error rate).




- ### Python Files 
  - [`Python_Quantum_Superposition_Distribution_Generator_Demo.py`](https://github.com/J2304789/Quantum-Superposition-Distribution-Generator/blob/main/Python_Quantum_Superposition_Distribution_Generator/Python_Quantum_Superposition_Distribution_Generator_Demo.py) is a demonstration on why a given percentage controlled rotation about the y axis would result in significant errors for values that are not located on any of the bases |0>,|+>,or |1>;the function <code>Quantum_Superposition_Distribution_Demo(_Prob_Value_)</code> can be utilized to provide a histogram of all possible measurement values based on specified Quantum Superposition Distribution. 
  
  - [`Python_Quantum_Superposition_Distribution_Generator_Polynomial.py`](https://github.com/J2304789/Quantum-Superposition-Distribution-Generator/blob/main/Python_Quantum_Superposition_Distribution_Generator/Python_Quantum_Superposition_Distribution_Generator_Polynomial.py) utilizes a polynomial function in order to scale the controlled rotations by a given percentage. However, because the values are predicted by a polynomial equation, they are highly inaccurate and are therefore left as a proof of concept (+/-95% error rate on both very low and very high numbers; average +/-35% error rate) and not recommended for any project utilization; the function <code>Quantum_Superposition_Distribution_Polynomial(_Prob_Value_)</code> can be utilized to provide a histogram of all possible measurement values based on specified Quantum Superposition Distribution. 
 
  - [`Python_Quantum_Superposition_Distribution_Generator_Cubic.py`](https://github.com/J2304789/Quantum-Superposition-Distribution-Generator/blob/main/Python_Quantum_Superposition_Distribution_Generator/Python_Quantum_Superposition_Distribution_Generator_Cubic.py) utilizes a Cubic function in order to scale the controlled rotations by a given percentage. However, because the values are predicted by a Cubic equation, they are highly inaccurate and are therefore left as a proof of concept (+/-80% error rate on both very low and very high numbers; average +/-30% error rate) and not recommended for any project utilization;;the function <code>Quantum_Superposition_Distribution_Cubic(_Prob_Value_)</code> can be utilized to provide a histogram of all possible measurement values based on specified Quantum Superposition Distribution. 
 
  
  - [`Python_Quantum_Superposition_Distribution_Generator_Quadratic.py`](https://github.com/J2304789/Quantum-Superposition-Distribution-Generator/blob/main/Python_Quantum_Superposition_Distribution_Generator/Python_Quantum_Superposition_Distribution_Generator_Quadratic.py) utilizes a Quadratic function in order to scale the controlled rotations by a given percentage. However, because the values are predicted by a Quadratic equation, they are highly inaccurate and are therefore left as a proof of concept (+/-80% error rate on both very low and very high numbers; average +/-20% error rate) and not recommended for any project utilization;the function <code>Quantum_Superposition_Distribution_Quadratic(_Prob_Value_)</code> can be utilized to provide a histogram of all possible measurement values based on specified Quantum Superposition Distribution. 
  - [`Python_Quantum_Superposition_Distribution_Generator_Quintic.py`](https://github.com/J2304789/Quantum-Superposition-Distribution-Generator/blob/main/Python_Quantum_Superposition_Distribution_Generator/Python_Quantum_Superposition_Distribution_Generator_Quintic.py) utilizes a Quintic function in order to scale the controlled rotations by a given percentage (+/-2% error rate on both very low and very high numbers; average +/-.5% error rate);;the function <code>Quantum_Superposition_Distribution_Quintic(_Prob_Value_)</code> can be utilized to provide a histogram of all possible measurement values based on specified Quantum Superposition Distribution. 

- ### Excel Files

  - [`Excel_Quantum_Superposition_Distribution_Generator_Calculation.xslx`](https://github.com/J2304789/Quantum-Superposition-Distribution-Generator/blob/main/Excel_Quantum_Superposition_Distribution_Generator/Excel_Quantum_Superposition_Distribution_Generator_Calculation.xlsx) utilizes Excel's Trendline function in order to generate an Polynomial equation to predict the controlled rotations.
 
  - #### Juypter Notebook
      - [`Excel_Juypter_Notebook_Polynomial.ipynb`](https://github.com/J2304789/Quantum-Superposition-Distribution-Generator/blob/main/Excel_Quantum_Superposition_Distribution_Generator/Excel_Juypter_Notebook_Quantum_Superposition_Distribution_Generator/Excel_Juypter_Notebook_Polynomial.ipynb) utilizes a polynomial function generated by Excel's Trendline function in order to scale the controlled rotations by a given percentage(+/-2% error rate on both very low and very high numbers; average +/-1% error rate)
 
    - [`Excel_Juypter_Notebook_Cubic.ipynb`](https://github.com/J2304789/Quantum-Superposition-Distribution-Generator/blob/main/Excel_Quantum_Superposition_Distribution_Generator/Excel_Juypter_Notebook_Quantum_Superposition_Distribution_Generator/Excel_Juypter_Notebook_Cubic.ipynb) utilizes a Cubic function generated by Excel's Trendline function in order to scale the controlled rotations by a given percentage(+/-1% error rate on both very low and very high numbers; average +/-.3% error rate)

  
    - [`Excel_Juypter_Notebook_Quadratic.ipynb`](https://github.com/J2304789/Quantum-Superposition-Distribution-Generator/blob/main/Excel_Quantum_Superposition_Distribution_Generator/Excel_Juypter_Notebook_Quantum_Superposition_Distribution_Generator/Excel_Juypter_Notebook_Quadratic.ipynb) utilizes a Quadratic function generated by Excel's Trendline function in order to scale the controlled rotations by a given percentage(+/-80% error rate on very high numbers; average +/-6% error rate)
    
    - [`Excel_Juypter_Notebook_Quintic.ipynb`](https://github.com/J2304789/Quantum-Superposition-Distribution-Generator/blob/main/Excel_Quantum_Superposition_Distribution_Generator/Excel_Juypter_Notebook_Quantum_Superposition_Distribution_Generator/Excel_Juypter_Notebook_Quintic.ipynb) utilizes a Quintic function generated by Excel's Trendline function in order to scale the controlled rotations by a given percentage(+/-4% error rate on both very low and very high numbers; average +/-3% error rate)
  
  - #### Python
       - [`Excel_Python_Polynomial.py`](https://github.com/J2304789/Quantum-Superposition-Distribution-Generator/blob/main/Excel_Quantum_Superposition_Distribution_Generator/Excel_Python_Quantum_Superposition_Distribution_Generator/Excel_Python_Polynomial.py) utilizes a polynomial function generated by Excel's Trendline function in order to scale the controlled rotations by a given percentage(+/-2% error rate on both very low and very high numbers; average +/-1% error rate);the function <code>Excel_Quantum_Superposition_Distribution_Polynomial(_Prob_Value_)</code> can be utilized to provide a histogram of all possible measurement values based on specified Quantum Superposition Distribution. 
 
    - [`Excel_Python_Cubic.py`](https://github.com/J2304789/Quantum-Superposition-Distribution-Generator/blob/main/Excel_Quantum_Superposition_Distribution_Generator/Excel_Python_Quantum_Superposition_Distribution_Generator/Excel_Python_Cubic.py) utilizes a Cubic function generated by Excel's Trendline function in order to scale the controlled rotations by a given percentage(+/-1% error rate on both very low and very high numbers; average +/-.3% error rate);the function <code>Excel_Quantum_Superposition_Distribution_Cubic(_Prob_Value_)</code> can be utilized to provide a histogram of all possible measurement values based on specified Quantum Superposition Distribution.

  
    - [`Excel_Python_Quadratic.py`](https://github.com/J2304789/Quantum-Superposition-Distribution-Generator/blob/main/Excel_Quantum_Superposition_Distribution_Generator/Excel_Python_Quantum_Superposition_Distribution_Generator/Excel_Python_Quadratic.py) utilizes a Quadratic function generated by Excel's Trendline function in order to scale the controlled rotations by a given percentage(+/-80% error rate on very high numbers; average +/-6% error rate);the function <code>Excel_Quantum_Superposition_Distribution_Quadratic(_Prob_Value_)</code> can be utilized to provide a histogram of all possible measurement values based on specified Quantum Superposition Distribution.
    
    - [`Excel_Python_Quintic.py`](https://github.com/J2304789/Quantum-Superposition-Distribution-Generator/blob/main/Excel_Quantum_Superposition_Distribution_Generator/Excel_Python_Quantum_Superposition_Distribution_Generator/Excel_Python_Quintic.py) utilizes a Quintic function generated by Excel's Trendline function in order to scale the controlled rotations by a given percentage(+/-4% error rate on both very low and very high numbers; average +/-3% error rate);the function <code>Excel_Quantum_Superposition_Distribution_Quintic(_Prob_Value_)</code> can be utilized to provide a histogram of all possible measurement values based on specified Quantum Superposition Distribution.

## 🗒 Notes
- ### Juypter Notebook

  - Activate following code in Juypter notebook files in order to graph Qubit Bloch spheres:

```
qc.save_statevector()
qobj=assemble(qc)
result=sim.run(qobj).result().get_statevector()
plot_bloch_multivector(result)
``` 

- ### Python 
  - Import either <code>Quantum_Superposition_Distribution_Demo(_Prob_Value_)</code> , <code>Quantum_Superposition_Distribution_Polynomial(_Prob_Value_)</code>, <code>Quantum_Superposition_Distribution_Cubic(_Prob_Value_)</code>,<code>Quantum_Superposition_Distribution_Quadratic(_Prob_Value_)</code>, or <code>Quantum_Superposition_Distribution_Quintic(_Prob_Value_)</code> from [`Python_Quantum_Superposition_Distribution_Generator_Demo.ipynb`](https://github.com/J2304789/Quantum-Superposition-Distribution-Generator/blob/main/Python_Quantum_Superposition_Distribution_Generator/Python_Quantum_Superposition_Distribution_Generator_Demo.py), [`Python_Quantum_Superposition_Distribution_Generator_Polynomial.ipynb`](https://github.com/J2304789/Quantum-Superposition-Distribution-Generator/blob/main/Python_Quantum_Superposition_Distribution_Generator/Python_Quantum_Superposition_Distribution_Generator_Polynomial.py),[`Python_Quantum_Superposition_Distribution_Generator_Cubic.ipynb`](https://github.com/J2304789/Quantum-Superposition-Distribution-Generator/blob/main/Python_Quantum_Superposition_Distribution_Generator/Python_Quantum_Superposition_Distribution_Generator_Cubic.py), [`Python_Quantum_Superposition_Distribution_Generator_Quadratic.ipynb`](https://github.com/J2304789/Quantum-Superposition-Distribution-Generator/blob/main/Python_Quantum_Superposition_Distribution_Generator/Python_Quantum_Superposition_Distribution_Generator_Quadratic.py),or [`Python_Quantum_Superposition_Distribution_Generator_Quintic.ipynb`](https://github.com/J2304789/Quantum-Superposition-Distribution-Generator/blob/main/Python_Quantum_Superposition_Distribution_Generator/Python_Quantum_Superposition_Distribution_Generator_Quintic.py) respectively.

-  ### Excel
   - Import either <code>Excel_Quantum_Superposition_Distribution_Polynomial(_Prob_Value_)</code> , <code>Excel_Quantum_Superposition_Distribution_Cubic(_Prob_Value_)</code>,<br><code>Excel_Quantum_Superposition_Distribution_Quadratic(_Prob_Value_)</code>, or <code>Excel_Quantum_Superposition_Distribution_Quintic(_Prob_Value_)</code> from [`Excel_Juypter_Notebook_Polynomial.ipynb`](https://github.com/J2304789/Quantum-Superposition-Distribution-Generator/blob/main/Excel_Quantum_Superposition_Distribution_Generator/Excel_Python_Quantum_Superposition_Distribution_Generator/Excel_Python_Polynomial.py), [`Excel_Python_Cubic.ipynb`](https://github.com/J2304789/Quantum-Superposition-Distribution-Generator/blob/main/Excel_Quantum_Superposition_Distribution_Generator/Excel_Python_Quantum_Superposition_Distribution_Generator/Excel_Python_Cubic.py),[`Excel_Python_Quadratic.ipynb`](https://github.com/J2304789/Quantum-Superposition-Distribution-Generator/blob/main/Excel_Quantum_Superposition_Distribution_Generator/Excel_Python_Quantum_Superposition_Distribution_Generator/Excel_Python_Quadratic.py) or [`Excel_Python_Quintic.ipynb`](https://github.com/J2304789/Quantum-Superposition-Distribution-Generator/blob/main/Excel_Quantum_Superposition_Distribution_Generator/Excel_Python_Quantum_Superposition_Distribution_Generator/Excel_Python_Quintic.py) respectively.
