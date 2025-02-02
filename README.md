  # Telegram Commerce Copilot 🤖🛍️  

An AI-powered shopping assistant for Telegram that enables natural language product discovery, visual search, and automated commerce workflows.  

## Tech Stack 🛠️  

### **Core**  
`Python 3.10` `Django 4.2` `PostgreSQL` `Redis` `Celery`  

### **AI**  
`Sentence Transformers` `OpenCV` `ResNet50`  

### **Infra**  
`Docker` `Gunicorn` `Nginx`  

### **Frontend**  
`Vue.js 3` `Chart.js` `Telegram Bot API`  

## Features ✨  

- **🤖 AI-Powered Product Search**  
  Natural language understanding for queries like _"Show me blue dresses under $50"_.  

- **📸 Image-Based Visual Search**  
  Find similar products using photo uploads.  

- **🔔 Real-Time Notifications**  
  Price drop alerts and restock updates via **n8n workflows**.  

- **📊 Admin Dashboard**  
  Vue.js interface for monitoring user engagement and sales metrics.  

- **🚀 Production-Ready**  
  Dockerized microservices with load-balanced Kubernetes deployment.  

## Installation 📦  

### **Clone repository**  
```sh  
git clone https://github.com/yourusername/telegram-commerce-copilot.git  
```  

### **Start services**  
```sh  
docker-compose up --build  
```  

## Configuration ⚙️  

Set these environment variables in `.env`:  

```ini  
TELEGRAM_BOT_TOKEN=<YOUR_BOT_TOKEN>  
DJANGO_SECRET_KEY=<YOUR_SECRET_KEY>  
DB_URL=postgres://user:pass@db:5432/main  
REDIS_URL=redis://redis:6379/0  
```  

## API Examples 💻  

### **Text Search Request**  
```sh  
curl -X POST http://localhost:8000/api/search \  
  -H "Content-Type: application/json" \  
  -d '{"query": "summer dresses under $50", "user_id": 123}'  
```  

### **Image Search Response**  
```json  
{  
  "results": [  
    {  
      "product_id": 456,  
      "name": "Blue Floral Sundress",  
      "price": 39.99,  
      "similarity_score": 0.92  
    }  
  ]  
}  
```  

## Contributing 🤝  

1. **Fork the repository**  
2. **Create a feature branch**  
   ```sh  
   git checkout -b feature/amazing-feature  
   ```  
3. **Commit changes**  
   ```sh  
   git commit -m 'Add amazing feature'  
   ```  
4. **Push to branch**  
   ```sh  
   git push origin feature/amazing-feature  
   ```  
5. **Open a Pull Request**  

## License 📄  

Distributed under the **MIT License**. See `LICENSE` for more information.  
