# cvxpy_benchmark
Benchmarking cvxpy with Airspeed Velocity.

- [airspeed velocity](https://asv.readthedocs.io/en/stable/index.html)

# Requirements

You need to install ``asv`` benchmark framework and ``virtualenv``.

    pip install asv virtualenv


# Usage

## 1. clone this repo, and move the repository dir.

    git clone https://github.com/AtsushiSakai/cvxpy_benchmark.git
    cd cvxpy_benchmark 

## 2. Do benchmarking

    asv run asv run --skip-existing-commits ALL
    
At first time of benchmarking, it takes a long time, because all commits are benchmarked.

From the second time, only new commits are benchmarked.

## 3. Show benchmark result

Generate html document

    asv publish
    
Open it in a web browser

    asv preview -b
    
# Sample benchmark reports

- [airspeed velocity of an unladen cvxpy](https://atsushisakai.github.io/cvxpy_benchmark/)

# Ref

- https://github.com/chainer/chainer-benchmark
