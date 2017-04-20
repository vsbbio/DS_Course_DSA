## [MatPlotLib]("http://matplotlib.org")

""" Data visualization"""

### Library:    import matplotlib.pyplot as plt
                %matplotlib inline => To show inside Jupyter notebook

### Building Std graphs

    

    1. plt.plot("data", label= String/Legend*, color = 'r/g/y') => To get axis and values
        e.g.:
            
            x = [1,2,3]
            y = [2,3,4]
            plt.plot(x, y)
            
        1a. plt.xlabe("Varíavel 1")  => To define the label
        1b. plt.ylabel("Varíavel 2") 
        1c. plt.title("Teste Plot") => Graph's name
        
    2.  plt.show() => To show the image
    3.  *plt.legend() => to show legend within graph (it need to define the label inside the function plt.plot)
    
### Other Options

    1. plt.plot("data", label= String/Legend*, color = 'r/g/y')
    2. plt.bar(data, label= String/Legend, color ='r')
    3. plt.hist(data=Max2, frequency, histtype = bar/stepfilled, rwidth = 0.8)
    4. plt.scatter(data/axis=Max2, label = , color = , marker='o/*', s=100)
    5. plt.stackplot(data=Max2+, color=)
    6. plt.pie(data=Max2+, labels= , color= , startangle = 90, shadow=True/False, explode=())
    
### Plt.figure() | PyLab (from pylab import *)

    1. figName = plt.figure()  #generic function
    2. axes = fiName.add_axes([0.1,0.1,0.8,0.8])
        
        2a. axes.plot(data=x, data=y, 'r')
        2b. axes.set_xlabel('x')
        2c. axes_set_ylabel('y')
        2d. axes.set_title("Gráfico de Linha")
        
### SubPlot

    1. fig, axes = plt.subplots(nrows=1, ncols=2)  ==> axes[0] and axes[1]
      
        1a. for ax in axes:
                ax.plot(x, y, 'r')
                ax.set_xlabel =('x')
                ax.set_ylabel = ('y')
                ax.set_title('foda-se')
                
            fig.tight_layout()
    2.  axes.axis('tight')
    3.  axes.set_x/ylim([0,60])
    4.  axes.set_yscale('log')
    5.  axes.grid(color=, alpha=, linestyle='dashed', linewidth=) or simples (True)

### 3D Graph - (from mpl_toolkits.mplot3d.axes3d import Axes3D)


    
    
        