init:
	@python3 -m venv .venv && \
		. .venv/bin/activate && \
		pip install -r requirements.txt && \
		pip install -e .

init-dev: init
	@. .venv/bin/activate && \
		pip install -r requirements-test.txt

format:
	@. .venv/bin/activate && \
		ruff format

check:
	@. .venv/bin/activate && \
		mypy . && \
		ruff check
