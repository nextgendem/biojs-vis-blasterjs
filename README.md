biojs-vis-blasterjs
=====

### Authors
* Aitor Blanco Míguez (aiblanco@uvigo.es)
* Dr. Anália Maria Garcia Lourenço (analia@uvigo.es)
* Dr. Borja Sánchez García (borja.sanchez@csic.es)
* Dr. Florentino Fernández Riverola (riverola@uvigo.es)

### Description 
[![NPM version](http://img.shields.io/npm/v/biojs-vis-blasterjs.svg)](https://www.npmjs.org/package/biojs-vis-blasterjs) 

> A free to use, open source Javascript BLAST alignments viewer library created by SING group.

### Requeriments
* Bootstrap 3 ([http://getbootstrap.com/])
* HTML2CANVAS ([http://html2canvas.hertzen.com/])

### Accepted files
BLAST output files -outfmt 0 (Default) 
> Only one query on the BLAST file.   
> You can check [NCBI BLAST user manual].

## Getting Started
Install the module with: `npm install biojs-vis-blasterjs`

```html
<head>
	<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/css/bootstrap.min.css" integrity="sha384-1q8mTJOASx8j1Au+a5WDVnPi2lkFfwwEAa8hDDdjZlpLegxhjVME1fgjWPGmkzs7" crossorigin="anonymous" />
    ...
</head>
<body>
    ...
    <input type="file" id="blastinput" />
    <div id="blast-multiple-alignments"></div>
    <div id="blast-alignments-table"></div>
    <div id="blast-single-alignment"></div>
    ...
    <script type="text/javascript" src="js/html2canvas.js"></script>    
    <script type="text/javascript">
      var blasterjs = require("biojs-vis-blasterjs");
      var instance = new blasterjs({
         input: "blastinput",
         multipleAlignments: "blast-multiple-alignments",
         alignmentsTable: "blast-alignments-table",
         singleAlignment: "blast-single-alignment"
      });
    </script>
</body>
```

### Institution
[© SING - Sistemas Informáticos de Nueva Generación 2015]    
Department of Computer Science, University of Vigo    
ESEI - Escuela Superior de Ingeniería Informática Edificio politécnico    
Campus Universitario As Lagoas s/n    
32004 Ourense, Spain    
Tel: +34 988 387 013    
Fax: +34 988 387 001

## Contributing
All contributions are welcome.

## Support
If you have any problem or suggestion please open an issue [here](https://github.com/sing-group/biojs-vis-blasterjs/issues).

### TODOs

- Accept more blast output formats.

## License 
[GNU General Public License v3]

BlasterJS is a free to use, open source JS library created by SING Group.
Copyright (C) 2016  SING - Sistemas Informaticos de Nueva Generacion

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.


   [http://getbootstrap.com/]: <http://getbootstrap.com/>
   [https://html2canvas.hertzen.com/]: <https://html2canvas.hertzen.com/>
   [© SING - Sistemas Informáticos de Nueva Generación 2015]: <http://sing.ei.uvigo.es/>
   [NCBI BLAST user manual]: <http://www.ncbi.nlm.nih.gov/books/NBK279675/>
   [GNU General Public License v3]: <https://github.com/sing-group/biojs-vis-blasterjs/blob/master/LICENSE>
