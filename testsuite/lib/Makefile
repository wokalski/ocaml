#**************************************************************************
#*                                                                        *
#*                                 OCaml                                  *
#*                                                                        *
#*                 Xavier Clerc, SED, INRIA Rocquencourt                  *
#*                                                                        *
#*   Copyright 2010 Institut National de Recherche en Informatique et     *
#*     en Automatique.                                                    *
#*                                                                        *
#*   All rights reserved.  This file is distributed under the terms of    *
#*   the GNU Lesser General Public License version 2.1, with the          *
#*   special exception on linking described in the file LICENSE.          *
#*                                                                        *
#**************************************************************************

.PHONY: compile
compile: compile-targets

.PHONY: promote
promote: defaultpromote

.PHONY: clean
clean: defaultclean

include ../makefiles/Makefile.common

.PHONY: compile-targets
compile-targets: testing.cmi testing.cmo
	@if $(BYTECODE_ONLY); then : ; else \
	  $(MAKE) testing.cmx; \
	fi
