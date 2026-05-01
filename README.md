readme
prueba
name: Pull Request Workflow

on: pull_request

jobs:
  pr-job:
    runs-on: ubuntu-latest
    steps:
      - name: Info del PR
        run: |
          echo "🔁 Se ejecutó con un PULL REQUEST"
          echo "Autor: ${{ github.actor }}"
          echo "Rama origen: ${{ github.head_ref }}"
          echo "Rama destino: ${{ github.base_ref }}"
