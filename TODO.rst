cfanalytics 
-----------

TODO list
=========

Code
----
- Update ``Cfopendata`` example and create a ``Clean`` example. 
- Write documentation for online and eventually run the examples in the docs.
- ``Cfplot(df).cityplot()`` Could add state input to stop picking up other states or look for the most popular like you did for countries https://github.com/raybellwaves/cfanalytics/blob/master/cfanalytics/core/cfplot.py#L1064

Data
----
- Backfill data before 2017. Can then track an athlete's percentile over the years or a the maximum score/P50 for a repeated workout in various years.

Analysis/plotting
-----------------
- Create distribution plots of scores using `seaborn <https://seaborn.pydata.org/>`__ as ``Cfplot(df).distplot(column=‘18.1_score’)``. I'm guessing the results will look like a `Rayleigh <https://en.wikipedia.org/wiki/Rayleigh_distribution>`__ distribution.
- Create interactive plots of scores using `bokeh <https://bokeh.pydata.org/en/latest/>`__ / `holoviews <http://holoviews.org/>`__. Would be cool if could query for a person on the plot may not be possible.
- Create interactive spatial plots using `geoviews <http://geo.holoviews.org/>`__. This may allow you to zoom in on individual gyms. Or do some fancy shit and plot the data on Google Earth. 
- Check out ``xarray``'s `API <https://github.com/pydata/xarray/tree/0d69bf9dbf281f0f0f48ac2fadda61a82533aac3/xarray/plot>`__ (and `docs <http://xarray.pydata.org/en/stable/plotting.html>`__) for how to code the plots. 
- ``Cfplot(df).pairplot(x='18.2_rank', y='18.2a_rank')``
