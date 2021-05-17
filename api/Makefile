

.PHONY: clone
clone:
     mkdir test
     cd test
     docker clone https://github.com/AsishVenakataSai/docker-test.git 
       
.PHONY: clean
clean:
     cd ..
     rm -f test
   
.PHONY: build
build: 
     mvn -B package --file pom.xml 
       
       
