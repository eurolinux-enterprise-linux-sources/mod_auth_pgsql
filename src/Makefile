APACHE2_HOME=/usr/local/apache2
PGSQL_LIB=/usr/local/pgsql/lib
PGSQL_INCLUDE=/usr/local/pgsql/include

shared:
	${APACHE2_HOME}/bin/apxs  -i -a -c -I ${PGSQL_INCLUDE} -L ${PGSQL_LIB} -lpq mod_auth_pgsql.c

indent:
	indent -kr -ts4 mod_auth_pgsql.c

clean:
	rm -rf .libs/ *.la *.o *.lo *.slo *~	