

include ../../../GDALmake.opt

OBJ	=	ogropenfilegdbdriver.o ogropenfilegdbdatasource.o ogropenfilegdblayer.o filegdbtable.o filegdbindex.o

CPPFLAGS	:=	-I.. -I../.. -I../mem $(GDAL_INCLUDE) $(CPPFLAGS)

default:	$(O_OBJ:.o=.$(OBJ_EXT))

clean:
	rm -f *.o $(O_OBJ)

$(O_OBJ):	ogr_openfilegdb.h filegdbtable.h filegdbtable_priv.h ../mem/ogr_mem.h
