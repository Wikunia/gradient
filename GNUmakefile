
build:
	jossy ./lib/gradient.js > gradient.js
	borschik -t js -i gradient.js -o gradient.min.js

test: build
	cp ./gradient.js ./tests/gradient.js
	coffee ./tests/gradient-test.coffee


.PHONY: build