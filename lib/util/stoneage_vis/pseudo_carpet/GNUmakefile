# -*- Mode: Makefile -*- 

## Define the variables needed by Make.example

# the base name(s) of the application(s) in this directory
ebase = pseudocarpet

# the location of Chombo lib dir
CHOMBO_HOME = ../../../

# names of Chombo libraries needed by this program, in order of search.
LibNames =   AMRTools LevelTools BoxTools

# relative paths to source code directories
base_dir = .
src_dirs = 

# input file for 'run' target
INPUT = ramp.inputs

# shared code for building example programs
include $(CHOMBO_HOME)/mk/Make.example

#sanity
#glliblocs = -L/usr/lib -L/usr/X11R6/lib 
#gllibs = -lglut -lGLU -lGL   
#glinclocs =  -I/usr/include/ -I/usr/X11/include
#spencer
glliblocs = -L$(HOME)/lib
glinclocs = -I$(HOME)/include
gllibs = -lglut -lMesaGLU -lMesaGL -L/usr/X11R6/lib -lX11 -lXext -lXmu -lXt -lXi -lSM -lICE  

XTRACXXFLAGS = $(glliblocs) $(glinclocs)
XTRALIBFLAGS = $(gllibs)
# application-specific variables

# Note: tell Make.rules to not use -q for 'run' target
_space = # # NOTE: keep the space after the "=" or bad things happen
VERBOSE = $(_space)

# application-specific targets

