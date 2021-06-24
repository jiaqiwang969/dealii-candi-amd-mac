# dealii-candi-amd-mac

- bug01: -lfortran error
"https://thecoatlessprofessor.com/programming/cpp/rcpp-rcpparmadillo-and-os-x-mavericks-lgfortran-and-lquadmath-error/"
the official gfortran binaries break the compile chain because the binaries listed were not used to compile R. As a result, using gfortran will lead you to switch from receiving a “-lgfortran” error to a “-lquadmath” error since a few files are missing from the expected locations.
  solution: 
  `brew install gcc@9`
  gcc-10 is not OK! 

  “https://github.com/fxcoudert/gfortran-for-macOS”

  r