# mlflow
#### Описание основных шагов
1) Создаем папку **mlflow-tutorial** и открываем ее в VS
2) Создаем виртуальное окружение **python3 -m venv .env**
3) Активируем виртуальное окружение **source .env/bin/active**
4) Создаем вспомогательную папку **mlflow**
5) Прописываем имя данной папки в переменных окружения **export MLFLOW_REGISTRY_URI=mlflow**
6) Запускаем сервер **mlflow server --backend-store-uri sqlite:///${MLFLOW_REGISTRY_URI}/mlruns.db --default-artifact-root ${MLFLOW_REGISTRY_URI} --host localhost --port 5000**
7) Формируем файл с необходимыми скриптами. В скриптах должна быть строчка  **mlflow.set_tracking_uri("http://localhost:5000")**
8) Конроль за экспериментами **http://127.0.0.1:5000 (http://localhost:5000)**

#### Дополнительный материал по теме
1) Проект Анастасии Никулиной https://github.com/miracl1e6/auto-pipeline-airflow-mlflow
2) Материал к вебинару "Пример использования автоматического логирования экспериментов в mlflow и mlflow models" (youtube канал Учебный центр "Коммерсант") https://gist.github.com/MachineLearningIsEasy/8614de5f3de88ec194b09d4d4c6d7c48



