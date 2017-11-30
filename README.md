<img src="https://github.com/di-unipi-socc/FogTorchPI/blob/master/img/logoftpi.PNG" width="300">

_A tool for probabilistic QoS-assurance, resource consumption and cost estimation of eligible deployments of Fog applications._

This version of FogTorchΠ exploits [Apache Maven](https://maven.apache.org/) building tool and json input. It is based upon the work described in

> [Antonio Brogi](http://pages.di.unipi.it/brogi), [Stefano Forti](http://pages.di.unipi.it/forti), [Ahmad Ibrahim](http://pages.di.unipi.it/ibrahim) <br>
> **Estimating QoS, resource consumption and cost of Fog application deployments.** <br>
> _Submitted to_ [Fog World Congress 2017 (FWC'17)](https://www.fogworldcongress.com/cfp), Oct. 30 – Nov. 1, 2017, Santa Clara, California

If you wish to reuse source code in this repo, please cite the above mentioned article.

# Example
After cloning the repo and installing Maven, it is sufficient to run 

```
mvn clean install
```
from the FogTorchΠ  folder to create an executable jar with all needed dependencies (viz., [gson](https://github.com/google/gson)). Then running the command

```
java -jar FogTorchPi-0.1-jar-with-dependencies.jar <input>.json <output>.csv
```

from the target folder, executes FogTorchΠ with the preset value of 100,000 simulations to estimate QoS-assurance, resource consumption and cost. 

A full input example is in file [input/FWC17_3G.json](https://github.com/di-unipi-socc/FogTorchPI/tree/costmodel/input/FWC17_3G.json) and [input/FWC17_4G.json](https://github.com/di-unipi-socc/FogTorchPI/tree/costmodel/input/FWC17_4G.json) and related results can be found in [results/FWC17](https://github.com/di-unipi-socc/FogTorchPI/tree/costmodel/results/FWC17), along with the Python script to plot the 3D visualisation.


