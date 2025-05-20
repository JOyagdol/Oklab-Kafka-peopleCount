# PeopleCount Kafka Consumer

🧍 Kafka 기반 인원 수 감지 시스템의 데이터 수신 및 처리 컴포넌트입니다.

## 📌 개요

이 Kafka Consumer는 사람 수 감지 센서나 영상 분석 시스템으로부터 전송되는 실시간 데이터를 수신하고, 이를 분석하여 특정 공간의 인원 수를 파악하거나 후속 시스템에 전달하는 역할을 합니다.

---

## 📦 주요 기능

- Kafka 토픽(`people-count-event`)
- JSON 기반 인원 수 데이터 파싱
- 데이터 정합성 검증
- 알림 시스템 연계 (Webhook / DB 저장 등)

---

## ⚙️ 시스템 구조

```
People Counter Producer (센서 or 영상분석)
        ↓
[Kafka Topic: people-count-event]
        ↓
PeopleCount Kafka Consumer
        ↓
[분석 및 저장 / 알림 연동]
```
