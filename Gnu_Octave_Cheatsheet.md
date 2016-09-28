# Logical operators

tilde 		NOT  
&& 		AND  
|| 		OR  

xor(3,8) 	XOR  

# Data types

numbers		3, 3.56  
string		'hello world'  
boolean		1 or 0  
Matrix 2x3	[44,55,66; 66,77,888]  



# Tricks and tips

A = 0: 2 : 10		% Create an array from 0 to 10 by mutiples of 2   
A = 0 : 10		% Create an array from 0 to 10    
ones(3,4)		% 3x4 ones matrix   
zeroes(3,4)		% 3x4 zeroes matrix   
rand(2,3)		% random martix 2,3   
eye(5)			% Identity matrix 5x5   
A(3,2)			% Get Matrix A's 3rd row 2nd column value
A(3,:)			% Get Matrix A's 3rd row every columns value  
A(:,2)			% Get Matrix A's every row from 2nd column values  
A(:)			% Create a column vector from matrix A  
C = [A, B]		% Concatanate matrix A and B to C. This is not matrix addition 
A * B			% Matrix multiplication
A .* B			% Element wise multiplication in matrix 
A .^2			% Element wise squaring
A .*2			% Element wise multiplication
A'			% Transpose of matrix A
pinv(A)			% Transpose of matrix A
magic(3)		% Creates a 3x3 magic matrix
find(A > 10)		% Return index numbers of items in matrix A, which satisy A > 10

help <<function-name>> 	% prints details about the function-name   
size(<matrix>)		% Returns diamentions of the <matrix>
pwd			% Prints current woriking directory  
cd '/go/to/directory'	% Goes to specified directory
ls			% Show items in the current woriking directory  
who 			% Shows vairables in current Octave session
whos			% Shows details of vairables in current Octave session
clear <variable-name>	% Clears variable from current Octave session
save <filename> <varname> % Saves varaible values to filename in current working directory
save <filename> <varname> -ascii % Saves varaible values in ASCII format

    
# Plotting data

plot(t,A)		% Plot t matrix on x axis, A matrix on y axis
plot(t,A, 'r')		% Plot t and A in red color
xlabel('name of x label') % Label x axis
ylabel('name of y label') % Label y axis
legend('name of legend')  % Add a legend to graph
title('Any title')	  % Add a title to the graph
hold on			% plot next graph on top of previous graph 
pring -dpng 'mygraph.png'	% Save garph to png format
subplot(1,2,1)		% Create a subplot with 1 row 2 columns, add next plot to first colomun
plot(t,A)		% This grapgh is added to 1 st column now
subplot(1,2,2)		% Create a subplot with 1 row 2 columns, add next plot to first colomun
plot(t,B)		% This grapgh is added to 2 nd column now
clf 			% clears a graph


