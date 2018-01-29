cmake_minimum_required (VERSION 2.6)
project (MODFLOW-USG-TRANSPORT)
enable_language( Fortran )
set( Toolchain gFortran )

file(GLOB mfusgt_src "*.f" "*.f90" )

add_executable(mfusgt ${mfusgt_src})

SET_TARGET_PROPERTIES(mfusgt PROPERTIES LINKER_LANGUAGE Fortran)
