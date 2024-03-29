# config_maker
Configuration Generator

## Usage

    ./config_maker -h
    
    USAGE: config_maker {-i | -t <config_template> | -f <csv_file> [-d <directory> | -o <file> | -c | -r <template_file>] | -h}

		-i			interactive mode - prompted interface
		-t <config_template>	template mode - import template with assigned variables
		-f <csv_file>		file mode - import data from .csv file
		    -d <directory>	   file mode - directory to write configuration files
		    -o <file>		   file mode - send all configuration to specified output file
		    -c			   file mode - concatenate output to existing file
		    -r <template_file>	   file mode - override template file from csv with specified template filen
		-h			help

## [TEMPLATE](a1.1.tmpl)
This file is the configuration.  This is a sample template file.

      a1.1.tmpl
  
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

### Interactive -i
The script will run in interactive mode if no paramaters or options are passed.  The script will prompt the user for the device_id.  This is the same name as the template file.  The script will then prompt for values for the variables defined in the header of the template file.

### Template -t
The script will run with the values defined for the variables in the template file itself.

### File -f [-d -o -c -r]
The script will pass in a .csv and populate the device_id (template file) as well as all variables.  Each variable in the template file should be a column of the .csv.  See [EXAMPLE CSV](sample.csv).
      
## Todo
See [TODO](TODO.md) for a list of planned features/fixes.

## Changelog
See [CHANGELOG](CHANGELOG.md) for a list of changes.
