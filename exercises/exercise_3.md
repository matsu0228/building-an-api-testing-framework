## Exercise 3 - fixtures
**Goal**: use fixtures for test setup and teardown  
**Purpose**: separate setup & teardown from the tests (separation of concerns,
don't repeat yourself)

### Assignment
Create a test using fixtures in which you:
- get a token
- create a book
- delete that book

### Fixtures
Pytest allows you to define fixtures for test setup and teardown using the
`@pytest.fixture` decorator. You can use the return value of a fixture in a test
by providing the name of the fixture as an argument to a test function.

Example:
```
import pytest

@pytest.fixture
def my_favourite_number():
    return 73
    
def test_my_favourite_number_is_73(my_favourite_number):
    assert my_favourite_number == 73
```

Note that not only tests can use fixtures, fixtures can also use other fixtures.

Docs: https://docs.pytest.org/en/latest/fixture.html