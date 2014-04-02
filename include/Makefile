
.PHONY: run_dev_ops run_dev_www

run_dev_ops: config-OPS_PORT
	echo "Run dev ops on port $(OPS_PORT)"

run_dev_www: config-WWW_PORT
	echo "Run dev www on port $(WWW_PORT)"

config-%:
	@if [ "${${*}}" == "" ]; then \
		echo "Config variable $* is not set, set the variable if you want to enable this command for your project"; \
		exit 1; \
	fi
