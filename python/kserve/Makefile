.PHONY: test

dev_install:
	poetry install --with test --extras "storage openai"

install_dependencies:
	poetry install --with=test --no-interaction --no-root --extras "storage openai"

test:
	cd ../ && pytest -W ignore kserve/test

type_check:
	mypy --ignore-missing-imports kserve
