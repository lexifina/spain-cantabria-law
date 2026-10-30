# Cantabria: law history in git

The law of the autonomous community of Cantabria (Comunidad Autónoma de Cantabria, Spain) as a git history: one file per article, one commit per norm that changed it, dated the day the change took effect, with the amending norm as the commit's author. `git blame` names the norm behind every paragraph; `git log` lists every change to an article; checking out a date gives the text in force that day.

It follows the shared design of [lexifina/global-law](https://github.com/lexifina/global-law), which places it at `es-cb/`. Spain's national law is in [lexifina/spain-law](https://github.com/lexifina/spain-law).

The text is in Spanish, exactly as the BOE's consolidated text prints it. Texts in co-official languages are not included.

Basado en datos de la Agencia Estatal Boletín Oficial del Estado (<https://www.boe.es>). Every text here is a consolidated text for information only (texto consolidado de carácter meramente informativo), not an official publication.

## What this repository holds

151 norms with 742 versions so far: the Estatuto de Autonomía first, then the laws, decree-laws and legislative decrees in force that the BOE consolidates, oldest first, added in parts of about 50. 13 of them are repealed norms the BOE consolidates: their whole history is kept, and their last commit removes the text on the day the repeal took effect, credited to the repealing norm. Regulations are not included (the BOE consolidates no autonomic decrees or orders).

| Folder | Norm | Versions | History | BOE last updated |
| --- | --- | ---: | --- | --- |
| `estatuto-de-autonomia/` | Ley Orgánica 8/1981, de 30 de diciembre, de Estatuto de Autonomía para Cantabria. | 8 | as first published, then each change: 31 January 1982 to 25 March 2021 | 2026-10-16 |
| `ley-1983-006/` | Ley 6/1983, de 4 de julio, sobre procedimiento para la designación de senador en representación de la Comunidad Autónoma de Cantabria. | 1 | oldest version available: 4 July 1983 | 2023-12-26 |
| `ley-1984-006/` | Ley 6/1984, de 29 de octubre, sobre protección y fomento de las especies forestales autóctonas. | 1 | as first published: 17 November 1984 | 2025-12-16 |
| `ley-1984-009/` | Ley 9/1984, de 22 de diciembre, de la Bandera de la Comunidad Autónoma de Cantabria. | 1 | as first published: 9 January 1985 | 2025-12-16 |
| `ley-1984-008/` | Ley 8/1984, de 22 de diciembre, del Escudo de la Comunidad Autónoma de Cantabria. | 1 | as first published: 10 January 1985 | 2025-12-16 |
| `ley-1985-010/` | Ley 10/1985, de 16 de diciembre, de Protección y Modernización de la Empresa Familiar Agraria. | 1 | oldest version available: 7 January 1986 | 2023-12-26 |
| `ley-1987-002/` | Ley 2/1987, de 6 de marzo, de Honores, Condecoraciones y Distinciones de la Diputación Regional de Cantabria. | 1 | as first published: 24 March 1987 | 2025-12-17 |
| `ley-1987-003/` | Ley 3/1987, de 6 de marzo, por la que se establece el Himno de Cantabria y se regula su uso. | 1 | as first published: 24 March 1987 | 2025-12-17 |
| `ley-1987-005/` | Ley 5/1987, de 27 de marzo, de Elecciones a la Asamblea Regional de Cantabria. | 6 | as first published, then each change: 4 April 1987 to 9 March 2019 | 2025-12-17 |
| `ley-1987-004/` | Ley 4/1987, de 27 de marzo, de uso conjunto de la bandera y escudo de la Comunidad Autónoma de Cantabria. | 1 | as first published: 7 April 1987 | 2025-12-17 |
| `ley-1988-002/` | Ley 2/1988, de 26 de octubre, de fomento, ordenación y aprovechamiento de los balnearios y de las aguas mineromedicinales y/o termales de Cantabria. | 2 | oldest version available, then each change: 29 May 1990 to 22 November 1998 | 2025-12-17 |
| `ley-1988-004/` | Ley 4/1988, de 26 de octubre, por la que se declara «Oyambre» Parque Natural. | 2 | as first published, then each change: 21 November 1988 to 2 June 2006 | 2025-12-17 |
| `ley-1990-006/` | Ley 6/1990, de 21 de marzo, de Capacitación Agraria. | 1 | as first published: 10 April 1990 | 2025-12-17 |
| `ley-1990-004/` | Ley 4/1990, de 23 de marzo, sobre concentración parcelaria, conservación de obras, unidades mínimas de cultivo y fomento de explotaciones rentables. | 2 | as first published, then each change: 29 April 1990 to 21 November 2000 | 2025-12-17 |
| `ley-1991-006/` | Ley 6/1991, de 26 de abril, de creación del Centro de Investigación del Medio Ambiente. | 1 | as first published: 7 May 1991 | 2025-12-17 |
| `ley-de-cantabria-1992-003/` | Ley de Cantabria 3/1992, de 18 de marzo, de Protección de los Animales. | 8 | as first published, then each change: 16 April 1992 to 1 January 2014 | 2026-04-28 |
| `ley-1992-008/` | Ley 8/1992, de 16 de diciembre, para la determinación de la capitalidad de los partidos judiciales de la Comunidad Autónoma de Cantabria. | 1 | as first published: 29 December 1992 | 2025-12-17 |
| `ley-de-cantabria-1992-009/` | Ley de Cantabria 9/1992, de 18 de diciembre, de Tasas y Precios Públicos de la Diputación Regional de Cantabria. | 36 | as first published, then each change: 31 December 1992 to 1 May 2026 | 2026-05-18 |
| `ley-de-cantabria-1993-004/` | Ley de Cantabria 4/1993, de 10 de marzo, de Función Pública. | 32 | as first published, then each change: 21 April 1993 to 12 November 2022 | 2026-04-29 |
| `ley-1993-005/` | Ley 5/1993, de 6 de mayo, de Presupuestos Generales de la Diputación Regional de Cantabria para 1993. | 8 | as first published, then each change: 5 July 1993 to 1 January 2018 | 2026-01-15 |
| `ley-1993-008/` | Ley 8/1993, de 18 de noviembre, del Plan de Gestión de Residuos Sólidos Urbanos de Cantabria. | 3 | as first published, then each change: 4 December 1993 to 1 January 2010 | 2025-12-17 |
| `ley-1994-002/` | Ley 2/1994, de 27 de enero, reguladora de los programas operativos de la Comunidad Autónoma de Cantabria, dentro del marco comunitario de apoyo. | 1 | as first published: 4 February 1994 | 2025-12-17 |
| `ley-1996-001/` | Ley 1/1996, de 14 de mayo, de Salud Mental de Cantabria. | 1 | as first published: 25 May 1996 | 2025-12-18 |
| `ley-1996-005/` | Ley 5/1996, de 17 de diciembre, de Carreteras de Cantabria. | 8 | as first published, then each change: 14 January 1997 to 1 May 2026 | 2026-05-14 |
| `ley-de-cantabria-1997-005/` | Ley de Cantabria 5/1997, de 6 de octubre, de Prevención, Asistencia e Incorporación Social en Materia de Drogodependencias. | 4 | as first published, then each change: 15 November 1997 to 1 January 2023 | 2026-04-29 |
| `ley-1997-007/` | Ley 7/1997, de 30 de diciembre, de Medidas Fiscales y Administrativas. | 4 | as first published, then each change: 1 January 1998 to 1 January 2020 | 2025-12-18 |
| `ley-1998-002/` | Ley 2/1998, de 6 de febrero, de creación del Colegio Profesional de Protésicos Dentales de Cantabria. | 1 | as first published: 14 February 1998 | 2025-12-18 |
| `ley-1998-007/` | Ley 7/1998, de 5 de junio, de Artesanía de Cantabria. | 2 | as first published, then each change: 25 June 1998 to 5 April 2025 | 2025-12-18 |
| `ley-1998-008/` | Ley 8/1998, de 12 de junio, de Creación del Colegio Profesional de Podólogos de Cantabria. | 1 | as first published: 30 June 1998 | 2025-12-18 |
| `ley-1998-009/` | Ley 9/1998, de 12 de junio, de Creación del Colegio Profesional de Fisioterapeutas de Cantabria. | 1 | as first published: 30 June 1998 | 2025-12-18 |
| `ley-1998-011/` | Ley 11/1998, de 13 de octubre, de Patrimonio Cultural de Cantabria. | 10 | as first published, then each change: 22 December 1998 to 29 August 2026 | 2026-08-10 |
| `ley-1999-001/` | Ley 1/1999, de 18 de febrero, de Declaración de Parque Natural de Collados del Asón. | 1 | as first published: 20 February 1999 | 2026-01-15 |
| `ley-1999-003/` | Ley 3/1999, de 24 de marzo, de Consejos Escolares de Cantabria. | 2 | as first published, then each change: 26 March 1999 to 1 January 2009 | 2026-01-15 |
| `ley-1999-005/` | Ley 5/1999, de 24 de marzo, de Ordenación del Turismo de Cantabria. | 10 | as first published, then each change: 26 March 1999 to 1 January 2025 | 2026-01-15 |
| `ley-1999-008/` | Ley 8/1999, de 28 de abril, de Comarcas de la Comunidad Autónoma de Cantabria. | 1 | as first published: 7 May 1999 | 2025-12-18 |
| `ley-1999-011/` | Ley 11/1999, de 27 de diciembre, de Medidas Fiscales y Administrativas. | 2 | as first published, then each change: 1 January 2000 to 1 January 2002 | 2025-12-18 |
| `ley-2000-002/` | Ley 2/2000, de 3 de julio, del Deporte. | 6 | as first published, then each change: 12 July 2000 to 1 January 2022 | 2025-12-18 |
| `ley-2000-003/` | Ley 3/2000, de 24 de julio, por la que se crea el Organismo Autónomo "Oficina de Calidad Alimentaria" (ODECA). | 2 | as first published, then each change: 3 November 2000 to 1 January 2008 | 2025-12-18 |
| `ley-2000-004/` | Ley 4/2000, de 13 de noviembre, de Modernización y Desarrollo Agrario. | 6 | oldest version available, then each change: 21 November 2000 to 1 January 2023 | 2025-12-18 |
| `ley-2001-001/` | Ley 1/2001, de 16 de marzo, de Colegios Profesionales de Cantabria. | 7 | as first published, then each change: 15 April 2001 to 1 January 2023 | 2026-06-26 |
| `ley-2001-003/` | Ley 3/2001, de 25 de septiembre, de Bibliotecas de Cantabria. | 1 | as first published: 3 December 2001 | 2025-12-18 |
| `ley-2001-005/` | Ley 5/2001, de 19 de noviembre, de Museos de Cantabria. | 2 | as first published, then each change: 29 November 2001 to 1 January 2018 | 2025-12-18 |
| `ley-2001-007/` | Ley 7/2001, de 19 de diciembre, de Ordenación Farmacéutica de Cantabria. | 8 | as first published, then each change: 16 January 2002 to 1 January 2023 | 2025-12-18 |
| `ley-2001-010/` | Ley 10/2001, de 28 de diciembre, de Creación del Servicio Cántabro de Salud. | 9 | as first published, then each change: 1 January 2002 to 1 May 2026 | 2026-05-14 |
| `ley-2002-001/` | Ley 1/2002, de 26 de febrero, del Comercio de Cantabria. | 10 | as first published, then each change: 7 March 2002 to 1 January 2018 | 2025-12-18 |
| `ley-2002-003/` | Ley 3/2002, de 28 de junio, de Archivos de Cantabria. | 1 | as first published: 29 July 2002 | 2026-04-21 |
| `ley-2002-005/` | Ley 5/2002, de 24 de julio, de Medidas Cautelares Urbanísticas en el ámbito del litoral, de sometimiento de los instrumentos de planificación territorial y urbanística a evaluación ambiental y de régimen urbanístico de los cementerios. | 3 | as first published, then each change: 2 August 2002 to 22 December 2006 | 2025-12-18 |
| `ley-2002-007/` | Ley 7/2002, de 10 de diciembre, de Ordenación Sanitaria de Cantabria. | 17 | as first published, then each change: 19 December 2002 to 1 May 2026 | 2026-05-14 |
| `ley-2003-001/` | Ley 1/2003, de 18 de marzo, de creación del Servicio Cántabro de Empleo. | 8 | as first published, then each change: 27 March 2003 to 1 January 2024 | 2025-12-18 |
| `ley-2003-002/` | Ley 2/2003, de 23 de julio, de establecimiento de medidas cautelares urbanísticas en el ámbito del litoral y creación de la Comisión Regional de Ordenación del Territorio y Urbanismo. | 1 | as first published: 2 August 2003 | 2025-12-18 |
| `ley-2004-001/` | Ley 1/2004, de 1 de abril, Integral para la Prevención de la Violencia Contra las Mujeres y la Protección a sus Víctimas. | 2 | as first published, then each change: 13 April 2004 to 28 January 2011 | 2025-12-18 |
| `ley-2004-002/` | Ley 2/2004, de 27 de septiembre, del Plan de Ordenación del Litoral. | 10 | as first published, then each change: 28 October 2004 to 5 April 2025 | 2025-12-18 |
| `ley-2004-003/` | Ley 3/2004, de 7 de octubre, de Creación del Colegio Profesional de Logopedas de Cantabria. | 1 | as first published: 19 October 2004 | 2025-12-18 |
| `ley-2004-005/` | Ley 5/2004, de 16 de noviembre, de Puertos de Cantabria. | 13 | as first published, then each change: 25 November 2004 to 1 January 2022 | 2025-12-18 |
| `ley-2005-001/` | Ley 1/2005, de 16 de mayo, de parejas de hecho de la Comunidad Autónoma de Cantabria. | 4 | as first published, then each change: 25 May 2005 to 1 January 2024 | 2025-12-18 |
| `ley-2005-002/` | Ley 2/2005, de 16 de junio, de creación del Colegio Profesional de Joyeros, Orfebres, Relojeros y Gemólogos de Cantabria. | 1 | as first published: 25 June 2005 | 2025-12-18 |
| `ley-2005-004/` | Ley 4/2005, de 5 de octubre, de estadística de Cantabria. | 2 | as first published, then each change: 6 November 2005 to 1 January 2021 | 2025-12-18 |
| `ley-2006-001/` | Ley 1/2006, de 7 de marzo, de Defensa de los Consumidores y Usuarios. | 13 | as first published, then each change: 15 May 2006 to 1 January 2024 | 2025-12-18 |
| `ley-2006-003/` | Ley 3/2006, de 18 de abril, del Patrimonio de la Comunidad Autónoma de Cantabria. | 12 | as first published, then each change: 28 April 2006 to 5 April 2025 | 2025-12-18 |
| `ley-2006-004/` | Ley 4/2006, de 19 de mayo, de Conservación de la Naturaleza de Cantabria. | 6 | as first published, then each change: 2 June 2006 to 5 April 2025 | 2025-12-18 |
| `ley-2006-006/` | Ley 6/2006, de 9 de junio, de prevención de la Contaminación Lumínica. | 1 | as first published: 16 September 2006 | 2025-12-18 |
| `ley-2006-007/` | Ley 7/2006, de 15 de junio, de garantías de tiempos máximos de respuesta en atención sanitaria especializada en el sistema sanitario público de Cantabria. | 1 | as first published: 23 June 2006 | 2025-12-18 |
| `ley-2006-010/` | Ley 10/2006, de 17 de julio, de Subvenciones de Cantabria. | 17 | as first published, then each change: 1 January 2007 to 1 May 2026 | 2026-05-14 |
| `ley-2006-011/` | Ley 11/2006, de 17 de julio, de organización y funcionamiento del Servicio Jurídico. | 7 | as first published, then each change: 1 August 2006 to 1 January 2023 | 2025-12-18 |
| `ley-2006-012/` | Ley 12/2006, de 17 de julio, de Caza de Cantabria. | 3 | as first published, then each change: 3 August 2006 to 3 June 2026 | 2026-06-10 |
| `ley-2006-014/` | Ley 14/2006, de 24 de octubre, de Finanzas de Cantabria. | 23 | as first published, then each change: 1 January 2007 to 5 April 2025 | 2026-05-08 |
| `ley-2006-016/` | Ley 16/2006, de 24 de octubre, de autorización del convenio de colaboración entre las Comunidades Autónomas de Cantabria, Castilla y León y el Principado de Asturias, para la gestión coordinada del Parque Nacional de los Picos de Europa. | 1 | as first published: 6 November 2006 | 2025-12-18 |
| `ley-2007-002/` | Ley 2/2007, de 27 de marzo, de derechos y servicios sociales. | 23 | as first published, then each change: 3 July 2007 to 5 June 2026 | 2026-06-05 |
| `ley-2007-003/` | Ley 3/2007, de 4 de abril, de Pesca en Aguas Continentales. | 2 | as first published, then each change: 18 April 2007 to 1 January 2014 | 2025-12-19 |
| `ley-2007-004/` | Ley 4/2007, de 4 de abril, de Cooperación Internacional al Desarrollo de la Comunidad Autónoma de Cantabria. | 2 | as first published, then each change: 18 April 2007 to 1 January 2013 | 2025-12-19 |
| `decreto-legislativo-2008-062/` | Decreto Legislativo 62/2008, de 19 de junio, por el que se aprueba el texto refundido de la Ley de Medidas Fiscales en materia de Tributos cedidos por el Estado. | 23 | oldest version available, then each change: 3 July 2008 to 1 May 2026 | 2026-05-14 |
| `ley-2008-001/` | Ley 1/2008, de 2 de julio, reguladora de los conflictos de intereses de los Miembros del Gobierno y de los Altos Cargos de la Administración de Cantabria. | 4 | as first published, then each change: 10 July 2008 to 1 January 2019 | 2025-12-19 |
| `ley-2008-002/` | Ley 2/2008, de 11 de julio, por la que se crea el Instituto de Finanzas de Cantabria. | 14 | as first published, then each change: 14 August 2008 to 1 May 2026 | 2026-05-14 |
| `ley-2008-004/` | Ley 4/2008, de 24 de noviembre, por la que se crea la Agencia Cántabra de Administración Tributaria. | 3 | as first published, then each change: 3 December 2008 to 1 January 2022 | 2025-12-19 |
| `ley-2008-005/` | Ley 5/2008, de 19 de diciembre, de creación del Instituto Cántabro de Seguridad y Salud en el Trabajo. | 4 | as first published, then each change: 31 December 2008 to 1 May 2026 | 2026-05-14 |
| `ley-2008-006/` | Ley 6/2008, de 26 de diciembre, de Educación de Cantabria. | 1 | as first published: 13 February 2009 | 2025-12-19 |
| `ley-2009-003/` | Ley 3/2009, de 27 de noviembre, de creación del Instituto Cántabro de Servicios Sociales. | 7 | as first published, then each change: 24 December 2009 to 1 January 2024 | 2025-12-19 |
| `ley-2009-004/` | Ley 4/2009, de 1 de diciembre, de participación institucional de los Agentes Sociales en el ámbito de la Comunidad Autónoma. | 3 | as first published, then each change: 25 December 2009 to 1 January 2019 | 2025-12-19 |
| `ley-2009-006/` | Ley 6/2009, de 28 de diciembre, de Medidas Fiscales y de Contenido Financiero. | 4 | oldest version available, then each change: 1 January 2010 to 1 January 2023 | 2025-12-19 |
| `ley-2010-004/` | Ley 4/2010, de 6 de julio, de educación en el tiempo libre. | 3 | as first published, then each change: 15 January 2011 to 5 April 2025 | 2025-12-19 |
| `ley-2010-006/` | Ley 6/2010, de 30 de julio, de Medidas urgentes en materia de Ordenación del Territorio y Urbanismo. | 2 | as first published, then each change: 13 August 2010 to 19 December 2012 | 2025-12-19 |
| `ley-2010-008/` | Ley 8/2010, de 23 de diciembre, de garantía de derechos y atención a la infancia y la adolescencia. | 6 | as first published, then each change: 28 January 2011 to 1 January 2023 | 2025-12-19 |
| `ley-2010-009/` | Ley 9/2010, de 23 de diciembre, de personal estatutario de instituciones sanitarias de la Comunidad Autónoma de Cantabria. | 15 | as first published, then each change: 28 January 2011 to 1 May 2026 | 2026-05-14 |
| `ley-2011-001/` | Ley 1/2011, de 28 de marzo, de Mediación de la Comunidad Autónoma de Cantabria. | 2 | as first published, then each change: 5 May 2011 to 28 April 2017 | 2025-12-19 |
| `ley-2012-002/` | Ley 2/2012, de 30 de mayo, de Medidas Administrativas, Económicas y Financieras para la ejecución del Plan de Sostenibilidad de los Servicios Públicos de la Comunidad Autónoma de Cantabria. | 14 | as first published, then each change: 2 June 2012 to 1 May 2026 | 2026-05-14 |
| `ley-2012-004/` | Ley 4/2012, de 15 de octubre, de Creación de la Contribución Especial por el establecimiento, mejora y ampliación de los Servicios de Prevención y Extinción de Incendios y de Salvamento de Cantabria. | 2 | as first published, then each change: 20 October 2012 to 1 January 2023 | 2025-12-19 |
| `ley-2012-008/` | Ley 8/2012, de 21 de diciembre, de Transporte de Personas por Cable. | 1 | as first published: 29 December 2012 | 2025-12-19 |
| `ley-2013-005/` | Ley 5/2013, de 5 de julio, por la que se reconoce como universidad privada a la Universidad Europea del Atlántico. | 1 | as first published: 16 July 2013 | 2025-12-19 |
| `ley-2013-006/` | Ley 6/2013, de 6 de noviembre, de Cooperativas de Cantabria. | 4 | as first published, then each change: 18 January 2014 to 5 April 2025 | 2025-12-19 |
| `ley-2013-007/` | Ley 7/2013, de 25 de noviembre, por la que se regula el aprovechamiento eólico en la Comunidad Autónoma de Cantabria. | 2 | as first published, then each change: 17 July 2014 to 1 January 2015 | 2025-12-19 |
| `ley-2014-001/` | Ley 1/2014, de 17 de noviembre, de Transporte de Viajeros por Carretera. | 5 | as first published, then each change: 2 December 2014 to 16 July 2026 | 2026-07-07 |
| `ley-2014-002/` | Ley 2/2014, de 26 de noviembre, de Abastecimiento y Saneamiento de Aguas de la Comunidad Autónoma de Cantabria. | 9 | as first published, then each change: 5 December 2014 to 5 April 2025 | 2025-12-19 |
| `ley-2014-004/` | Ley 4/2014, de 22 de diciembre, del Paisaje. | 1 | as first published: 29 January 2015 | 2025-12-19 |
| `ley-2014-005/` | Ley 5/2014, de 26 de diciembre, de Vivienda Protegida de Cantabria. | 8 | as first published, then each change: 30 December 2014 to 5 April 2025 | 2025-12-19 |
| `ley-2015-004/` | Ley 4/2015, de 23 de noviembre, de Creación del Colegio Profesional de Dietistas-Nutricionistas de Cantabria. | 1 | as first published: 2 December 2015 | 2025-12-19 |
| `ley-2015-006/` | Ley 6/2015, de 28 de diciembre, de Medidas Fiscales y Administrativas. | 2 | as first published, then each change: 1 January 2016 to 1 January 2021 | 2025-12-19 |
| `ley-2016-001/` | Ley 1/2016, de 28 de enero, de Creación del Colegio Profesional de Ingenieros Técnicos en Informática de Cantabria. | 1 | as first published: 5 February 2016 | 2025-12-19 |
| `ley-2016-002/` | Ley 2/2016, de 28 de enero, de Creación del Colegio Profesional de Ingenieros en Informática de Cantabria. | 1 | as first published: 5 February 2016 | 2025-12-19 |
| `ley-2016-004/` | Ley 4/2016, de 11 de noviembre, de creación del Colegio Profesional de Educadoras y Educadores sociales de Cantabria. | 1 | as first published: 22 November 2016 | 2025-12-19 |
| `ley-2017-003/` | Ley 3/2017, de 5 de abril, de Espectáculos Públicos y Actividades Recreativas de Cantabria. | 4 | as first published, then each change: 19 April 2017 to 1 January 2024 | 2025-12-19 |
| `ley-2017-006/` | Ley 6/2017, de 5 de julio, de acceso al entorno de personas con discapacidad que precisan el acompañamiento de perros de asistencia. | 1 | as first published: 15 July 2017 | 2025-12-19 |
| `ley-2018-001/` | Ley 1/2018, de 21 de marzo, de Transparencia de la Actividad Pública. | 5 | as first published, then each change: 29 September 2018 to 13 January 2026 | 2026-04-09 |
| `ley-2018-002/` | Ley 2/2018, de 8 de mayo, de Casas de Cantabria. | 1 | as first published: 18 May 2018 | 2025-12-20 |
| `ley-2018-003/` | Ley 3/2018, de 28 de mayo, de creación del Consejo de la Mujer. | 3 | as first published, then each change: 6 June 2018 to 5 April 2025 | 2025-12-20 |
| `ley-2018-004/` | Ley 4/2018, de 15 de junio, por el que se regula el Consejo Social de la Universidad de Cantabria. | 1 | as first published: 28 June 2018 | 2025-12-20 |
| `ley-2018-005/` | Ley 5/2018, de 22 de noviembre, de Régimen Jurídico del Gobierno, de la Administración y del Sector Público Institucional de la Comunidad Autónoma de Cantabria. | 11 | as first published, then each change: 3 January 2019 to 29 August 2026 | 2026-08-11 |
| `ley-2018-006/` | Ley 6/2018, de 22 de noviembre, por el que se crea el Organismo Autónomo Servicio de Emergencias de Cantabria. | 4 | as first published, then each change: 11 December 2018 to 21 November 2021 | 2025-12-20 |
| `ley-2018-007/` | Ley 7/2018, de 5 de diciembre, de Iniciativa Legislativa Popular de Cantabria. | 1 | as first published: 20 December 2018 | 2025-12-20 |
| `ley-2018-008/` | Ley 8/2018, de 11 de diciembre, del Consejo Económico y Social de Cantabria. | 3 | as first published, then each change: 1 July 2019 to 1 January 2021 | 2025-12-20 |
| `ley-2018-009/` | Ley 9/2018, de 21 de diciembre, de Garantía de los Derechos de las Personas con Discapacidad. | 3 | as first published, then each change: 12 January 2019 to 1 January 2025 | 2025-12-20 |
| `ley-2019-001/` | Ley 1/2019, de 14 de febrero, de creación del Consejo de la Juventud de Cantabria. | 3 | as first published, then each change: 26 February 2019 to 1 January 2024 | 2025-12-20 |
| `ley-2019-002/` | Ley 2/2019, de 7 de marzo, para la igualdad efectiva entre mujeres y hombres. | 3 | oldest version available, then each change: 9 March 2019 to 1 January 2024 | 2026-03-02 |
| `ley-2019-003/` | Ley 3/2019, de 8 de abril, del Sistema de Protección Civil y Gestión de Emergencias de Cantabria. | 3 | as first published, then each change: 17 April 2019 to 1 May 2026 | 2026-05-14 |
| `ley-2020-002/` | Ley 2/2020, de 28 de mayo, de concesión de ayudas económicas para mejorar las rentas de personas trabajadoras afectadas por expedientes de regulación temporal de empleo en el contexto de la crisis ocasionada por la pandemia de COVID-19. | 2 | oldest version available, then each change: 28 May 2020 to 1 January 2024 | 2025-12-20 |
| `ley-2020-004/` | Ley 4/2020, de 24 de junio, de creación del Colegio Profesional de Periodistas de Cantabria. | 1 | as first published: 2 July 2020 | 2026-03-02 |
| `ley-2020-005/` | Ley 5/2020, de 15 de julio, Reguladora del Fondo de Cooperación Municipal de Cantabria. | 1 | as first published: 25 July 2020 | 2025-12-20 |
| `ley-2020-006/` | Ley 6/2020, de 15 de julio, de Fundaciones de Cantabria. | 3 | as first published, then each change: 4 August 2020 to 5 April 2025 | 2026-02-24 |
| `ley-2020-007/` | Ley 7/2020, de 2 de octubre, de modificación de la Ley 3/2017, de 5 de abril, de Espectáculos Públicos y Actividades Recreativas de Cantabria. | 1 | as first published: 2 October 2020 | 2025-12-20 |
| `ley-2020-008/` | Ley 8/2020, de 11 de noviembre, de Garantía de Derechos de las Personas Lesbianas, Gais, Trans, Transgénero, Bisexuales e Intersexuales y No Discriminación por Razón de Orientación Sexual e Identidad de Género. | 1 | as first published: 9 December 2020 | 2025-12-20 |
| `ley-2021-001/` | Ley 1/2021, de 4 de marzo, de Pesca Marítima, Marisqueo y Acuicultura de Cantabria. | 2 | as first published, then each change: 22 April 2021 to 1 January 2022 | 2025-12-20 |
| `ley-2021-002/` | Ley 2/2021, de 28 de abril, por la que se declara el Parque Natural de las Dunas de Liencres y Costa Quebrada. | 1 | as first published: 7 May 2021 | 2025-12-20 |
| `ley-2021-004/` | Ley 4/2021, de 13 de mayo, de Regulación y Coordinación de los Servicios de Prevención, Extinción de Incendios y Salvamento de la Comunidad Autónoma. | 1 | as first published: 21 November 2021 | 2025-12-20 |
| `ley-2021-007/` | Ley 7/2021, de 5 de julio, por la que se extingue la Cámara Agraria de Cantabria. | 1 | as first published: 13 July 2021 | 2025-12-20 |
| `ley-2021-008/` | Ley 8/2021, de 17 de noviembre, de Memoria Histórica y Democrática de Cantabria. | 4 | as first published, then each change: 25 November 2021 to 9 July 2025 | 2025-12-20 |
| `ley-2022-003/` | Ley 3/2022, de 14 de junio, de Entidades Locales Menores. | 2 | as first published, then each change: 22 June 2022 to 1 January 2023 | 2026-03-02 |
| `ley-2022-004/` | Ley 4/2022, de 24 de junio, de Regulación del Juego de Cantabria. | 1 | as first published: 2 July 2022 | 2025-12-20 |
| `ley-2022-005/` | Ley 5/2022, de 15 de julio, de Ordenación del Territorio y Urbanismo de Cantabria. | 7 | as first published, then each change: 23 July 2022 to 1 May 2026 | 2026-10-16 |
| `ley-2022-007/` | Ley 7/2022, de 3 de noviembre, de creación del Instituto Cántabro de Administración Pública "Rafael de la Sierra". | 2 | as first published, then each change: 12 November 2022 to 5 April 2025 | 2025-12-20 |
| `ley-2022-008/` | Ley 8/2022, de 27 de diciembre, de Ciencia, Tecnología e Innovación de Cantabria. | 2 | oldest version available, then each change: 24 January 2023 to 5 April 2025 | 2026-03-02 |
| `ley-2022-009/` | Ley 9/2022, de 27 de diciembre, de Coordinación de Policías Locales de Cantabria. | 3 | as first published, then each change: 5 January 2023 to 12 June 2026 | 2026-06-22 |
| `ley-2023-001/` | Ley 1/2023, de 5 de abril, de Reconocimiento, Homenaje, Memoria y Dignidad a las Víctimas del Terrorismo. | 4 | as first published, then each change: 15 April 2023 to 12 March 2026 | 2026-03-23 |
| `ley-2025-002/` | Ley 2/2025, de 2 de abril, de Simplificación Administrativa de Cantabria. | 3 | as first published, then each change: 5 April 2025 to 5 June 2026 | 2026-06-05 |
| `ley-2025-003/` | Ley 3/2025, de 30 de junio, de Políticas de Juventud de Cantabria. | 1 | as first published: 1 January 2026 | 2025-12-20 |
| `ley-2025-004/` | Ley 4/2025, de 9 de octubre, del Voluntariado de Cantabria. | 1 | as first published: 16 October 2025 | 2025-12-20 |
| `ley-2025-005/` | Ley 5/2025, de 9 de octubre, de creación del Colegio Profesional de Terapeutas Ocupacionales de Cantabria. | 1 | as first published: 16 October 2025 | 2025-12-20 |
| `ley-2026-001/` | Ley 1/2026, de 5 de enero, de Participación Ciudadana en la Administración de la Comunidad Autónoma de Cantabria. | 1 | oldest version available: 13 January 2026 | 2026-04-09 |
| `ley-2026-008/` | Ley 8/2026, de 23 de junio, de Ordenación del Transporte Marítimo de Cantabria. | 1 | as first published: 16 July 2026 | 2026-07-07 |
| `ley-de-cantabria-2026-009/` | Ley de Cantabria 9/2026, de 23 de julio, de Control Ambiental. | 1 | as first published: 29 August 2026 | 2026-08-10 |
| `ley-1985-006/` | Ley 6/1985, de 5 de julio, de Iniciativa Legislativa Popular. | 2 | as first published, then each change: 16 July 1985 to 20 December 2018; **repealed** 20 December 2018 by Ley 7/2018, de 5 de diciembre (BOE-A-2019-398) | 2025-12-16 |
| `ley-1986-005/` | Ley 5/1986, de 7 de julio, del Centro de Estudios de la Administración Pública Regional de Cantabria. | 6 | as first published, then each change: 26 July 1986 to 12 November 2022; **repealed** 12 November 2022 by Ley 7/2022, de 3 de noviembre (BOE-A-2022-20715) | 2025-12-17 |
| `ley-1994-006/` | Ley 6/1994, de 19 de mayo, reguladora de las Entidades Locales Menores. | 2 | as first published, then each change: 4 June 1994 to 22 June 2022; **repealed** 22 June 2022 by Ley 3/2022, de 14 de junio (BOE-A-2022-12386) | 2025-12-17 |
| `ley-1996-003/` | Ley 3/1996, de 24 de septiembre, sobre Accesibilidad y Supresión de Barreras Arquitectónicas, Urbanísticas y de la Comunicación. | 4 | as first published, then each change: 22 October 1996 to 12 January 2019; **repealed** 12 January 2019 by Ley 9/2018, de 21 de diciembre (BOE-A-2019-1630) | 2025-12-18 |
| `ley-1998-003/` | Ley 3/1998, de 2 de marzo, de la Cámara Agraria. | 2 | as first published, then each change: 18 March 1998 to 13 July 2021; **repealed** 13 July 2021 by Ley 7/2021, de 5 de julio (BOE-A-2021-12057) | 2025-12-18 |
| `ley-2001-002/` | Ley 2/2001, de 25 de junio, de Ordenación Territorial y Régimen Urbanístico del Suelo de Cantabria. | 30 | as first published, then each change: 4 September 2001 to 22 September 2022; **repealed** 22 September 2022 by Ley 5/2022, de 15 de julio (BOE-A-2022-13844) | 2025-12-18 |
| `ley-2002-002/` | Ley 2/2002, de 29 de abril, de Saneamiento y Depuración de las Aguas Residuales de la Comunidad Autónoma de Cantabria. | 15 | as first published, then each change: 8 May 2002 to 5 December 2014; **repealed** 5 December 2014 by Ley 2/2014, de 26 de noviembre (BOE-A-2014-13624) | 2025-12-18 |
| `ley-2002-006/` | Ley 6/2002, de 10 de diciembre, de Régimen Jurídico del Gobierno y de la Administración de la Comunidad Autónoma de Cantabria. | 20 | as first published, then each change: 18 January 2003 to 3 January 2019; **repealed** 3 January 2019 by Ley 5/2018, de 22 de noviembre (BOE-A-2018-17138) | 2025-12-18 |
| `ley-2006-015/` | Ley 15/2006, de 24 de octubre, de Juego de Cantabria. | 7 | as first published, then each change: 28 October 2006 to 2 July 2022; **repealed** 2 July 2022 by Ley 4/2022, de 24 de junio (BOE-A-2022-12387) | 2025-12-18 |
| `ley-2006-017/` | Ley 17/2006, de 11 de diciembre, de control ambiental integrado. | 17 | as first published, then each change: 22 December 2006 to 29 August 2026; **repealed** 29 August 2026 by Ley de Cantabria 9/2026, de 23 de julio (BOE-A-2026-17287) | 2026-08-28 |
| `ley-2007-001/` | Ley 1/2007, de 1 de marzo, de Protección Civil y Gestión de Emergencias de Cantabria. | 3 | as first published, then each change: 10 March 2007 to 17 April 2019; **repealed** 17 April 2019 by Ley 3/2019, de 8 de abril (BOE-A-2019-6771) | 2025-12-19 |
| `ley-2015-002/` | Ley 2/2015, de 1 de octubre, por la que se aprueba el régimen sancionador en materia de espectáculos públicos, actividades recreativas y establecimientos públicos en la Comunidad Autónoma de Cantabria. | 2 | as first published, then each change: 3 October 2015 to 19 April 2017; **repealed** 19 April 2017 by Ley 3/2017, de 5 de abril (BOE-A-2017-5043) | 2025-12-19 |
| `ley-2021-009/` | Ley 9/2021, de 20 de diciembre, del Plan Estadístico 2021-2024. | 2 | as first published, then each change: 30 December 2021 to 27 March 2025; **repealed** 27 March 2025 by Ley 1/2025, de 19 de marzo (BOE-A-2025-6951) | 2025-12-20 |

## Source

The consolidated legislation of the Agencia Estatal Boletín Oficial del Estado (BOE), through its open-data API, <https://www.boe.es/datosabiertos/api/legislacion-consolidada>. For each consolidated norm it gives every block of the text (article, disposition, annex, heading) with every version of that block, the day each version took effect (fecha_vigencia) and the norm that made it (id_norma). Each version here is the whole text as it stood on one of those days. The last column above is the BOE's own last-update date for the consolidated text.

## Dates

- Each commit is dated at **noon, Europe/Madrid, on the day the change took effect**: the fecha_vigencia the BOE gives the new block versions.
- A day on which the BOE records a new block version that changes no words is not a version here.
- Block versions with no in-force date (the BOE's 99999999, a date not yet fixed) are left out.
- An act's first commit is its first publication when the BOE's earliest text is the act as enacted; otherwise it is the oldest version the BOE holds.
- Versions that take effect after the retrieval day are on the `futuro` branch, never merged into `main`.

## Files

`<act>/art-005.md` is Artículo 5, `art-005-bis.md` Artículo 5 bis; `da-01.md` the Disposición adicional primera, `dt-` transitional, `dd-` repealing and `df-` final dispositions (`-unica` for "única"); `preambulo.md` the preamble, `firma.md` the signature, `anexo-*.md` the annexes. The book, title, chapter and section headings sit at the top of the file of the article that follows them. One paragraph per line; a table one line per row, cells separated by ` | `.

## How it is checked

- Every version of every act is read back from git on the day it took effect and on the day before (`tools/check_repo.py`); both must match `corpus.json`.
- The letters and digits of every version equal those of the BOE's own text of that day, rebuilt from the source XML by a separate reader, and every file's text appears in it.
- Health checks: no merge commits, commit dates never go backwards, nothing dated in the future, and every commit's trailers parse.

## What "author" means

The author of a commit is the norm that changed the text (a law, a decree-law, a ruling of the Constitutional Court), named by its title and BOE identifier, with an e-mail address that cannot exist (`<boe id>@boe.es.invalid`). The committer is always Lexifina.

## Limits

This is not an official publication. Only the texts published in the official journals are authentic. The history starts with the oldest text the BOE consolidates for each norm. Only the norms listed above are included; norms the BOE does not consolidate are not.
