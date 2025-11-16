# Stability-Analysis-using-Bode-Plot
## Aim:
To analyse the stability of the system having open loop transfer function, G(S)=1/(S(1+0.5S)(1+0.1S)) using bode plot and verify it using MATLAB. 
## Apparatus Required:
Computer with MATLAB software

## Theory:



## Procedure:
	Open MATLAB software
	Open a new script file.
	Type the program.
	Save and Execute the program.
	Determine the gain crossover frequency, phase cross over frequency, gain margin and phase margin.
	Also determine the stability.

## Program: 
num = 1<br>
den = [0.05 0.6 1 0]<br>
sys = tf(num, den)<br>
bode(sys)<br>
grid on<br>
[Gm Pm Wpc Wgc] = margin(sys)<br>
if (Wpc > Wgc)<br>
    disp('stable')<br>
elseif (Wpc == Wgc)<br>
    disp('marginally stable')<br>
else<br>
    disp('unstable')<br>
end<br>


## Output:
<img width="868" height="783" alt="image" src="https://github.com/user-attachments/assets/3e434071-48ef-4e5d-8a81-4d099ddd0b54" />

## Result:
Thus the bode plot for the given transfer function was drawn and verified using MATLAB. <br>
Gain margin =12 <br>
Phase Margin =60 <br>
Gain crossover frequency =0.907 <br>
Phase crossover frequency =4.4721 <br>
The system is stable
