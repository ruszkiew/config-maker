# config_maker
Configuration Generator

## Usage

    ./config_maker -h
    
    USAGE: config_maker {-i | -f <csv_file> | -d <directory> | -t <config_template> | -h}

	-i			              interactive mode - prompted interface
		-t <config_template>	template mode - import template with assigned variables
		-f <csv_file>		file mode - import data from .csv file
		-d <directory>		   file mode - directory to write configuration files
		   -o <file>		   file mode - send all configuration to specified output file
		   -c			   file mode - concatenate output to existing file
		   -r <template_file>	   file mode - override template file from csv with specified template filen
	-h	help

## [TEMPLATE](a1.1.tmpl)
This file is the configuration.
      e.g. (a.1.1.tmpl)
  
Each template has a standard header.  The header
maintains the file name, description, file last updated,
file updated by, and release notes.


## [CONSTANT](constant.def)
This file represents constant values that can be referenced in a tempalte file.

    constant.def

## [VARIABLE](variable.def)

    variable.def

This file represents declared variables that can be referenced in a tempalte file.  Each variable can be validated with a regular expression.

## Script Modes

### Interactive

### Template

### File
      
## Examples

## Todo
See [TODO](TODO.md) for a list of planned features/fixes.

## Changelog
See [CHANGELOG](CHANGELOG.md) for a list of changes.
