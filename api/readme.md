
# 🧪 Loanstax Mock API – cURL Guide

Base URL:  
`https://australia-southeast1-finstack-ai.cloudfunctions.net/demoApi`

---

## 📍 1. Get Borrower Pipeline

```bash
curl -X GET https://australia-southeast1-finstack-ai.cloudfunctions.net/demoApi/api/borrowers/pipeline
```

---

## 📍 2. Get Borrower Detail

```bash
curl -X GET https://australia-southeast1-finstack-ai.cloudfunctions.net/demoApi/api/borrowers/ID12345
```

---

## 📍 3. Request Documents

```bash
curl -X POST https://australia-southeast1-finstack-ai.cloudfunctions.net/demoApi/api/borrowers/ID12345/request-documents \
  -H "Content-Type: application/json" \
  -d '{
    "success": true,
    "message": "Documents requested."
  }'
```

---

## 📍 4. Send to Valuer

```bash
curl -X POST https://australia-southeast1-finstack-ai.cloudfunctions.net/demoApi/api/borrowers/ID12345/send-valuer \
  -H "Content-Type: application/json" \
  -d '{
    "success": true,
    "message": "Valuer notified."
  }'
```

---

## 📍 5. Approve Loan

```bash
curl -X POST https://australia-southeast1-finstack-ai.cloudfunctions.net/demoApi/api/borrowers/ID12345/approve \
  -H "Content-Type: application/json" \
  -d '{
    "success": true,
    "message": "Loan approved."
  }'
```

---

## 📍 6. Escalate to Credit Committee

```bash
curl -X POST https://australia-southeast1-finstack-ai.cloudfunctions.net/demoApi/api/borrowers/ID12345/escalate \
  -H "Content-Type: application/json" \
  -d '{
    "success": true,
    "message": "Escalated to Credit Committee."
  }'
```

---

## 📍 7. Get Broker Info

```bash
curl -X GET https://australia-southeast1-finstack-ai.cloudfunctions.net/demoApi/api/broker/BROKER123
```

---

## 📍 8. Get Onboarding Workflow

```bash
curl -X GET https://australia-southeast1-finstack-ai.cloudfunctions.net/demoApi/api/onboarding/workflow
```

---

> 📝 Replace placeholder values like `ID12345` and `BROKER123` with real/mock IDs as needed.
