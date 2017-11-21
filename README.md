# fonts-automated-testing
This project help to test fonts rendering by using harfbuzz.

* src/generate_test.py
	This file is used to create {fontname}-std-test.txt. This is reference file with expected rendering of fonts with harfbuzz.

* src/auto_test.py
	This is file uses {fontname}-std-test.txt and updated fonts. It passes all the test cases with modified font to harfbuzz and check it with reference rendering and report issues with failed test cases.


## How to contribute
* Select fonts for automated test cases.
* Create list of characters/string to be tested. Good to have as many as you can.
* Check manually whether all the test cases working well before creating reference file.
* Run src/generate_test.py with tests.txt (File created in step2) and fonts ttf file. Outfile will be {fontname}-std-test.txt
* Comming it to git.
* Each time after changes in font run src/auto_test.py with {fontname}-std-test.txt and updated fonts ttf file.
