CXX = gcc
CXXFLAGS = -O2

.PHONY: all

all: eddington-deprecated eddington-hashmap eddington-tree eddington

eddington-deprecated: eddington-deprecated.c
	$(CXX) $(CXXFLAGS) $< -o $@

eddington-hashmap: eddington-hashmap.c hashmap.c primes.c
	$(CXX) $(CXXFLAGS) $^ -o $@ -lm

eddington-tree: eddington-tree.c tree.c
	$(CXX) $(CXXFLAGS) $^ -o $@

eddington: eddington.c
	$(CXX) $(CXXFLAGS) $< -o $@
