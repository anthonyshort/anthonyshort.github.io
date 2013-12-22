build: install ./stylesheets/index.css ./stylesheets/components
	cd stylesheets && component build --copy
	cat stylesheets/build/build.css | myth | cleancss > stylesheets/build/build.min.css

install: ./stylesheets/component.json
	cd stylesheets && component install

clean:
	rm -r stylesheets/components stylesheets/build

PHONY: clean