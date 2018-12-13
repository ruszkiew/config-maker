# config_maker
Configuration Generator

## Usage

    ./config_maker -h
    
    USAGE: config_maker {-i | -f <csv_file> | -d <directory> | -t <config_template> | -h}

    	-i			              interactive mode - prompted interface
	    -t <config_template>	template mode - import template with assigned variables
	    -f <csv_file>		      file mode - import data from .csv file
	      -d <directory>	       file mode - directory to write configuration files
	      -o <file>		           file mode - send all configuration to specified output file
	      -c 			               file mode - concatenate output to existing file
	      -r <template_file>	   file mode - override template file from csv with specified template filen
    	-h			help

## TEMPLATE File e.g.(a1.1.tmpl)

## CONSTANT File (constant.def)
This file represents constant values that can be referenced in a tempalte file.

## VARIABLE File (variable.def)
This file represents declared variables that can be referenced in a tempalte file.  Each variable can be validated with a regular expression.

## Sript Modes

### Interactive

### Template

### File
      
## Examples

## Todo
See [TODO](TODO.md) for a list of planned features/fixes.

## Changelog
See [CHANGELOG](CHANGELOG.md) for a list of changes.
