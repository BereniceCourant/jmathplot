
```
Usage : jplot2d(data1,options,data2,options) or jplot3d(data1,options,data2,options) [data] is an array of numbers, [options] are related to previous [data] and should be :

 -t <SCATTER|LINE|BAR|HISTOGRAM2D(<integer h>)|HISTOGRAM3D(<integer h>,<integer k>)|GRID3D|CLOUD2D(<integer h>,<integer k>)|CLOUD3D(<integer h>,<integer k>,<integer l>)>    type of the plot
      SCATTER|LINE|BAR: each line of the ASCII file contains coordinates of one point.
      HISTOGRAM2D(<integer h>): ASCII file contains the 1D sample (i.e. m=1) to split in h slices.
      HISTOGRAM3D(<integer h>,<integer k>): ASCII file contains the 2D sample (i.e. m=2) to split in h*k slices (h slices on X axis and k slices on Y axis).
      GRID3D: ASCII file is a matrix, first row gives n X grid values, first column gives m Y grid values, other values are Z values.
      CLOUD2D(<integer h>,<integer k>): ASCII file contains the 2D sample (i.e. m=2) to split in h*k slices (h slices on X axis and k slices on Y axis), density of cloud corresponds to frequency of X-Y slice in given 2D sample.
      CLOUD3D(<integer h>,<integer k>,<integer l>): ASCII file contains the 3D sample (i.e. m=3) to split in h*k*l slices (h slices on X axis, k slices on Y axis, l slices on Y axis), density of cloud corresponds to frequency of X-Y-Z slice in given 3D sample.
  -n name    name of the plot
  -v <ASCII file (n,3|2)>    vector data to add to the plot
  -q<X|Y|Z>(<float Q>) <ASCII file (n,1)>    Q-quantile to add to the plot on <X|Y|Z> axis. Each line of the given ASCII file contains the value of quantile for probvability Q.
  -qP<X|Y|Z> <ASCII file (n,p)>    p-quantiles density to add to the plot on <X|Y|Z> axis. Each line of the given ASCII file contains p values.
  -qN<X|Y|Z> <ASCII file (n,1)>    Gaussian density to add to the plot on <X|Y|Z> axis. Each line of the given ASCII file contains a standard deviation.
```