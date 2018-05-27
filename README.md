# Desafío de clasificación de audio FreeSound

#### Librosa

[Librería](https://github.com/librosa/librosa) de análisis de audio en Python. Parece tener implementados algoritmos para actividades típicas como separación de componentes armónicos y percusivos, extraer tonalidades y otros.

Tiene buena [documentación](http://librosa.github.io/librosa/), notebooks de [ejemplos](http://nbviewer.jupyter.org/github/librosa/librosa/blob/master/examples/LibROSA%20demo.ipynb) extensos y desarrollo activoen [GitHub]. También refiere a los papers originales en caso de que consideremos útil reimplenentar alguna técnica.

El [paper](conference.scipy.org/proceedings/scipy2015/pdfs/brian_mcfee.pdf) de presentación de la librería es bastante espectacular

#### Definición de características

EL primer paso sería definir unas características interesantes. De lo que hablamos hoy, surge jugar con la construcción de features separados para los componentes armónicos y percusivos de los sonidos, para lo cual ya hay una función de referencia implementada en librosa [`hpss`](http://librosa.github.io/librosa/generated/librosa.decompose.hpss.html#librosa.decompose.hpss).

