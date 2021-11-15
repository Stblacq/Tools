## Usage
````
class MyBodePlotter(BodePlotter):
  def get_G_j_w(self, w):
        """G(s) = K/2s+100"""
        k = 1
        s = complex(0, w)
        g = k / 2*s +100
        return g
   def get_H_j_w(self, w):
        s = complex(0, w)
        h = s/10
        return h

plotter = MyBodePlotter()
plotter.get_bode_plot()
```