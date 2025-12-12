
Info.

This is an Ancient Greek morphosyntactic analyzer and parser. It parses declensions and conjugations. This version is a two-layer model using a hidden sigmoid layer, linear output layer with softmax, and cross-entropy loss fxn. This version only predicts verb voice conjugation.

Data set is the Opera Graecae Adnotada (OGA) corpus, 40MM Ancient Greek word tokens across 1,999 texts, not included here. See below.


Setup.

- unzip the main project folder.

- Download, move, and unzip into the above main proj folder: Opera Graeca Adnotata from Zenodo or GitHub. This is two main folders OGA-main (5.9MB)and opera_graeca_adnotata_v0.2.0 (66GB)
links:
	* https://zenodo.org/records/14206061
	* https://github.com/OperaGraecaAdnotata/OGA

- Create and activate a virtual environment.
	* Change into your new, cloned and unzipped project directory
	$cd /Users/admin/Desktop/Opera_Graeca_Verb_Parser

	* create venv
	$python3 -m venv .venv
	when starting again in future, skip this step and just activate

	* activate
	$source .venv/bin/activate

- install dependencies
	* $pip install -r requirements.txt

- set an environment variable OGA_ROOT to the correct directory path of the OGA on your machine.
	* make sure you're in the right dir $cd /Users/admin/Desktop/Opera_Graeca_Verb_Parser
	* $export OGA_ROOT=/Users/admin/Desktop/Opera_Graeca_Verb_Parser/opera_graeca_adnotata/opera_graeca_adnotata_v0.2.0
	* confirm with $python3 -c "import os; print(os.environ.get('OGA_ROOT'))"

- start jupyter
	* $jupyter notebook



Shutdown.

- exit
	* ctrl+c

- deactivate venv
	* $deactivate
