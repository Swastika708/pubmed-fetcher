# pubmed-fetcher
Overview

PubMed Fetcher is a Python CLI tool that fetches research papers from the PubMed API, identifies papers with authors affiliated with pharmaceutical or biotech companies, and saves the results in a CSV file.

Features

Fetches research papers based on a user-specified query.

Filters authors affiliated with non-academic institutions.

Saves results in a CSV file.

Command-line interface (CLI) with multiple options.

Uses Poetry for dependency management.

Well-structured, modular, and tested.

Installation

Prerequisites

Ensure you have Python (>=3.8) and Poetry installed.

Clone the Repository

git clone https://github.com/YOUR_USERNAME/pubmed-fetcher.git
cd pubmed-fetcher

Install Dependencies

poetry install

Usage

Basic Command

poetry run get-papers-list "cancer drug discovery"

Options

-h or --help: Display usage instructions.

-d or --debug: Enable debug mode to print extra details.

-f FILENAME or --file FILENAME: Save results to a specified CSV file.

Example:

poetry run get-papers-list "diabetes treatment" -f results.csv -d

Output Format

The output CSV contains:

PubmedID: Unique identifier for the paper.

Title: Title of the paper.

Publication Date: Date the paper was published.

Non-academic Author(s): Names of authors affiliated with non-academic institutions.

Company Affiliation(s): Names of pharmaceutical/biotech companies.

Corresponding Author Email: Email address of the corresponding author.

Development

Running Tests

pytest tests/

Publishing to TestPyPI (Bonus Step)

poetry build
poetry publish -r testpypi

Contributing

Fork the repository.

Create a feature branch (git checkout -b feature-name).

Commit changes (git commit -m "Add new feature").

Push to GitHub (git push origin feature-name).

Open a pull request.

License

This project is licensed under the MIT License.

