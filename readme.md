#Project Install Instructions

##install

1.clone
2.pip install -r requirements.txt

##Testing
1. pytest
2.pytest --pylint
3. pytest --pylint --cov

##Results
1. Pytest
pytest
============================= test session starts ==============================
platform darwin -- Python 3.9.12, pytest-8.0.0, pluggy-1.4.0 -- /Users/nehabiswal/WebSystemDev/homework2/myproject/venv/bin/python
cachedir: .pytest_cache
rootdir: /Users/nehabiswal/WebSystemDev/homework2
configfile: pytest.ini
testpaths: tests
plugins: pylint-0.21.0, cov-4.1.0
collected 2 items                                                              

tests/test_calculator.py::test_addition PASSED                           [ 50%]
tests/test_calculator.py::test_subtraction PASSED                        [100%]

============================== 2 passed in 0.02s ==========

2. Pytest --pylint
pytest --pylint
============================= test session starts ==============================
platform darwin -- Python 3.9.12, pytest-8.0.0, pluggy-1.4.0 -- /Users/nehabiswal/WebSystemDev/homework2/myproject/venv/bin/python
cachedir: .pytest_cache
rootdir: /Users/nehabiswal/WebSystemDev/homework2
configfile: pytest.ini
testpaths: tests
plugins: pylint-0.21.0, cov-4.1.0
collected 4 items                                                              
--------------------------------------------------------------------------------
Linting files
.......
--------------------------------------------------------------------------------

tests/__init__.py::PYLINT SKIPPED (file(s) previously passed pylint ...) [ 25%]
tests/test_calculator.py::PYLINT FAILED                                  [ 50%]
tests/test_calculator.py::test_addition PASSED                           [ 75%]
tests/test_calculator.py::test_subtraction PASSED                        [100%]

=================================== FAILURES ===================================
______________________ [pylint] tests/test_calculator.py _______________________
C: 11, 0: Trailing newlines (trailing-newlines)
=========================== short test summary info ============================
FAILED tests/test_calculator.py::PYLINT
==================== 1 failed, 2 passed, 1 skipped in 0.46s ====================
(venv) (base) Bharats-MacBook-Pro-2:homework2 nehabiswal$ 




3. Pytest --pylint --cov 
pytest --pylint --cov
============================= test session starts ==============================
platform darwin -- Python 3.9.12, pytest-8.0.0, pluggy-1.4.0 -- /Users/nehabiswal/WebSystemDev/homework2/myproject/venv/bin/python
cachedir: .pytest_cache
rootdir: /Users/nehabiswal/WebSystemDev/homework2
configfile: pytest.ini
testpaths: tests
plugins: pylint-0.21.0, cov-4.1.0
collected 4 items                                                              
--------------------------------------------------------------------------------
Linting files
.......
--------------------------------------------------------------------------------

tests/__init__.py::PYLINT SKIPPED (file(s) previously passed pylint ...) [ 25%]
tests/test_calculator.py::PYLINT FAILED                                  [ 50%]
tests/test_calculator.py::test_addition PASSED                           [ 75%]
tests/test_calculator.py::test_subtraction PASSED                        [100%]

=================================== FAILURES ===================================
______________________ [pylint] tests/test_calculator.py _______________________
C: 11, 0: Trailing newlines (trailing-newlines)

---------- coverage: platform darwin, python 3.9.12-final-0 ----------
Name                       Stmts   Miss  Cover
----------------------------------------------
calculator/__init__.py         4      0   100%
tests/__init__.py              0      0   100%
tests/test_calculator.py       5      0   100%
----------------------------------------------
TOTAL                          9      0   100%

=========================== short test summary info ============================
FAILED tests/test_calculator.py::PYLINT
==================== 1 failed, 2 passed, 1 skipped in 0.78s ====================
(venv) (base) Bharats-MacBook-Pro-2:homework2 nehabiswal$ 
 

