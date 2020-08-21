REV := ffbf2eff6e

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
