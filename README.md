# django-celery
Simple Django Project with Celery


# Run Redis Worker on Windows
celery -A proj worker --pool=solo -l INFO

# Run Celery Beat to assign Scheduled Tasks
celery -A proj beat -l INFO --scheduler django_celery_beat.schedulers:DatabaseScheduler