REV := 9c0908d5cc11a79aaa1352699c408ea0c7123eca

.PHONY: package
package: ./lexbor-c/build/liblexbor_static.a

./lexbor-c:
	git clone https://github.com/lexbor/lexbor.git ./lexbor-c
	cd lexbor-c && git reset --hard $(REV)

./lexbor-c/build/liblexbor_static.a: ./lexbor-c
	mkdir -p lexbor-c/build
	cp lxbMakefile lexbor-c/build/Makefile
	cd ./lexbor-c/build && make lexbor_static -j

.PHONY: clean
clean:
	rm -rf ./lexbor-c
