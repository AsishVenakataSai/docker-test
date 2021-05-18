.PHONY: configure
configure:
	git config --global user.name $(USERNAME)
	git config --global user.email $(MAILID)
.PHONY: build
build:
	mkdir TEST
	cd TEST
	mkdir $(PROJECT)
	http://10.10.1.37/fractal/nsl-common-services.git
	git checkout $(BRANCH)
	cd logical-model
	mvn -B package --file pom.xml
.PHONY: copy
copy:
	cp ~/target/*.jar ~/lib/$(PROJECT)
	git add lib
	git commit -m "adding updated jar"
