# Einfaches-lineares-Regressionsmodell-mit-Pinguinen-Dataset

# Explore Linear Regression with Python

Dieses Notebook stammt aus einer Übung des Kurses **"The Power of Statistics"** im Rahmen des **Google Data Analytics Professional Certificate** auf **Coursera**, das ich aktuell absolviere.

## Ziel

Ziel der Übung ist es, den kompletten Workflow zum Aufbau eines **einfachen linearen Regressionsmodells** in Python nachzuvollziehen – von der Datenexploration über die Modellkonstruktion bis zur Überprüfung der Modellannahmen.

## Datensatz

Verwendet wird der in `seaborn` enthaltene **Penguins-Datensatz**. Für die Analyse werden nur die Arten *Adelie* und *Gentoo* berücksichtigt, fehlende Werte werden entfernt.

## Methode

1. **Explorative Datenanalyse (EDA):** Mithilfe von Pairplots werden lineare Zusammenhänge zwischen den numerischen Variablen (Schnabellänge, Schnabeltiefe, Flossenlänge, Körpermasse) identifiziert.
2. **Modellkonstruktion:** Mit `statsmodels.formula.api.ols()` wird ein einfaches lineares Regressionsmodell gebaut, das die Körpermasse (`body_mass_g`) anhand der Schnabellänge (`bill_length_mm`) vorhersagt.
3. **Überprüfung der Modellannahmen:**
   - **Linearität** anhand von Scatterplots
   - **Normalverteilung der Residuen** anhand eines Histogramms bzw. Q-Q-Plots
   - **Homoskedastizität** anhand eines Residuen-vs.-Fitted-Values-Plots

## Ergebnis

Das Modell zeigt einen deutlichen linearen Zusammenhang zwischen Schnabellänge und Körpermasse bei den betrachteten Pinguinarten und erfüllt die zentralen Annahmen der linearen Regression.

## Herkunft

Annotiertes Übungsnotebook aus dem Google Data Analytics Certificate (Coursera), Kurs "The Power of Statistics".
