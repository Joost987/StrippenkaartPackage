How to use this package: First begin a strippenkaart environment with \begin{strippenkaart}. An optional argument for the scale of the strippenkaart can be given, you can for example make the picture 2 times bigger by beginning with \begin{strippenkaart}[2].

Now add crossings with \kruising{1}{2} where the first argument is the amount of roads that should be kept on your left, and the second in the amount of roads that should be kept on your right. 
\kruisingstippel{1}{2}{3}{4} can also be used to make crossings with dashed lines. The first two arguments are still the amount of roads that should be kept to your left and right, the next two are how many of those lines you want to be dashed, again first for the left and then for the right. 

Next there is also \tekstbox{1}{2}, which adds a textbox at the current height, so next to the kruising defined directly above it. The first argument is the text you want to put in the textbox, the second argument is the x-coordinate of the box. Negative values mean to the left of the strippenkaart, positive to the right. The x-coordinate should have absolute value bigger than 2 if you do not want it to be inside of the strippenkaart.

Also, note that tikz is used for all the drawing and tikz is also supported inside of the strippenkaart environment. Therefore you can draw anything you want as well using tikz, but if you think it should be an extra feature please let me know.

Finally, end the environment with \end{strippenkaart}. 

An example.tex file is also included to show the usage of the commands


