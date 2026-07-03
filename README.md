# WhatsApp eCommerce Bot 🤖

Sistema de agente de ventas inteligente para dropshipping con integración a múltiples canales de comunicación y sincronización de inventario.

## 🚀 Características

- **Integración Multi-Canal**
  - ✅ WhatsApp Business API
  - ✅ Instagram Graph API
  - ✅ Facebook Messenger
  - ✅ TiendaNube eCommerce

- **Funcionalidades de eCommerce**
  - 🛍️ Catálogo de productos dinámico
  - 🛒 Carrito de compras
  - 💳 Procesamiento de pagos (Stripe)
  - 📦 Gestión de órdenes
  - 🔄 Sincronización con proveedores

- **Características del Bot**
  - 🤖 NLP básico para entender intenciones
  - 💬 Conversaciones naturales
  - 📱 Respuestas automáticas inteligentes
  - 📊 Analytics y reportes

## 📋 Requisitos Previos

- Node.js >= 18.0.0
- npm o yarn
- Cuentas y tokens de:
  - WhatsApp Business API
  - Meta/Facebook (Instagram, Messenger)
  - TiendaNube
  - Stripe (procesamiento de pagos)

## 🔧 Instalación

```bash
# Clonar repositorio
git clone https://github.com/lautarobutt/whatsapp-ecommerce-bot.git
cd whatsapp-ecommerce-bot

# Instalar dependencias
npm install

# Configurar variables de entorno
cp .env.example .env
# Editar .env con tus tokens y credenciales

# Build
npm run build

# Iniciar en desarrollo
npm run dev
```

## 📁 Estructura del Proyecto

```
whatsapp-ecommerce-bot/
├── src/
│   ├── index.ts
│   ├── config/
│   │   ├── environment.ts
│   │   └── integrations.ts
│   ├── channels/
│   │   ├── whatsapp/
│   │   ├── instagram/
│   │   ├── facebook/
│   │   └── base.channel.ts
│   ├── services/
│   │   ├── product.service.ts
│   │   ├── order.service.ts
│   │   ├── payment.service.ts
│   │   ├── cart.service.ts
│   │   └── tiendanube.service.ts
│   ├── models/
│   │   ├── product.model.ts
│   │   ├── order.model.ts
│   │   ├── user.model.ts
│   │   └── cart.model.ts
│   ├── middlewares/
│   │   ├── auth.middleware.ts
│   │   ├── validation.middleware.ts
│   │   └── error.middleware.ts
│   ├── utils/
│   │   ├── logger.ts
│   │   ├── formatters.ts
│   │   └── validators.ts
│   └── api/
│       └── routes.ts
├── tests/
├── docs/
├── .env.example
├── .gitignore
├── package.json
├── tsconfig.json
└── README.md
```

## 🔌 Configuración de Integraciones

### WhatsApp Business API

1. Registrarse en [Meta Business Platform](https://business.facebook.com)
2. Crear una aplicación WhatsApp Business
3. Obtener Phone ID y Access Token
4. Configurar webhook

### Instagram Graph API

1. Crear aplicación en Meta Developers
2. Configurar Instagram Business
3. Obtener Access Token

### Facebook Messenger

1. Crear página de Facebook
2. Conectar aplicación a la página
3. Generar Page Access Token

### TiendaNube

1. Registrarse en [TiendaNube](https://www.tiendanube.com)
2. Crear aplicación OAuth
3. Obtener Store ID y Access Token

## 📚 Documentación API

Ver documentación completa en `/docs`:
- [Configuración](docs/SETUP.md)
- [API Endpoints](docs/API.md)
- [Integraciones](docs/INTEGRATIONS.md)
- [Ejemplos de Uso](docs/EXAMPLES.md)

## 🧪 Testing

```bash
npm test
```

## 📝 Licencia

MIT

## 🤝 Contribuir

Las contribuciones son bienvenidas. Por favor:

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📧 Soporte

Para soporte, abre un issue en el repositorio.

## 🎯 Roadmap

- [ ] Dashboard de analytics
- [ ] Inteligencia artificial mejorada
- [ ] Soporte para más métodos de pago
- [ ] Integración con más plataformas de ecommerce
- [ ] Sistema de descuentos y promociones
- [ ] Chat en vivo con agentes humanos
