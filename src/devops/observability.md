# Observability


Observability (**наблюдаемость**) - это концепция, которая означает, насколько легко и эффективно вы можете наблюдать, измерять и понимать, что происходит внутри вашей системы. Это очень важно так как позволяет быстро обнаруживать, диагностировать и устранять проблемы, а также улучшать производительность и безопасность системы.

Можно выделить следующие направления:

1. **Логирование (Logging):**
   - Логирование - это процесс записи событий и данных о работе вашей системы в лог-файлы. Логи могут содержать информацию о действиях пользователя, ошибках, исключениях, запросах и других событиях.
   - Преимущества: Логи помогают выявлять и анализировать проблемы, воссоздавать сценарии ошибок и обеспечивать безопасность.
   - Популярные инструменты: Log4j, Logback, ELK Stack (Elasticsearch, Logstash, Kibana), Fluentd.
2. **Мониторинг (Monitoring):**
   - Мониторинг - это процесс наблюдения за состоянием системы в реальном времени. Он включает сбор и агрегацию метрик, таких как использование ресурсов, нагрузка на сервер и статус сервисов.
   - Преимущества: Мониторинг помогает оперативно обнаруживать и реагировать на проблемы, а также оптимизировать производительность системы.
   - Популярные инструменты: Prometheus, Grafana, Nagios, Zabbix.
3. **Алертинг(Alerting)**
   - Алертинг (Alerting) - это важная часть системы мониторинга и обеспечения надежности, которая позволяет оперативно реагировать на проблемы и уведомлять администраторов или инженеров о них.
   - Популярные инструменты: Prometheus Alertmanager, Grafana Alerting, Nagios, Zabbix и многие другие. Эти инструменты позволяют определять условия, при которых должно генерироваться уведомление.
   - **Триггеры и Условия (Triggers and Conditions):** Алерты создаются на основе заданных условий или триггеров. Например, условие может быть следующим: "Если использование процессора превышает 90% в течение 5 минут, сгенерировать алерт."
   - **Уровни Важности (Severity Levels):** Алерты могут иметь разные уровни важности, такие как информационные, предупреждающие, критические и т. д. Уровень важности определяет, насколько критична проблема.
   - **Уведомления (Notifications):** Системы алертинга интегрируются с различными каналами уведомления, такими как электронная почта, SMS, мессенджеры (Slack, Telegram), системы вызовов (PagerDuty) и другие. Когда алерт срабатывает, система отправляет уведомление на выбранный канал.
4. **Трейсинг (Tracing):**
   - Трейсинг - это метод изучения пути выполнения запроса через распределенную систему. Он позволяет отслеживать, какие компоненты обрабатывают запрос, и где возникают задержки.
   - Преимущества: Трейсинг упрощает обнаружение и устранение узких мест в производительности, а также улучшает отладку распределенных систем.
   - Популярные инструменты: Jaeger, Zipkin, OpenTelemetry.
5. **Профайлинг (Profiling):**
   - Профайлинг - это процесс анализа производительности приложения или системы, позволяющий выявить места, где приложение тратит больше всего времени.
   - Преимущества: Профайлинг позволяет оптимизировать производительность, выявлять "горячие" участки кода и улучшать архитектуру приложения.
   - Популярные инструменты: Go Profiler, pprof, Java Flight Recorder.