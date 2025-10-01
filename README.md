# País C - Colombia 🇨🇴

Aplicación Android para Colombia que utiliza los módulos compartidos de `repo-principal`.

## 🚀 Stack Tecnológico

- **Kotlin** 1.9.20
- **Jetpack Compose** - UI moderna
- **Android SDK** 34
- **Módulos compartidos**:
  - `shared-models` - Modelos de datos
  - `shared-components` - Componentes UI
  - `shared-screens` - Pantallas base

## 📦 Dependencias

Este proyecto depende de los módulos compartidos publicados desde `repo-principal`:

```kotlin
implementation("com.org:shared-models:1.0.0")
implementation("com.org:shared-components:1.0.0")
implementation("com.org:shared-screens:1.0.0")
```

## 🛠️ Configuración

### 1. Configurar GitHub Packages

Crea o edita `~/.gradle/gradle.properties`:

```properties
gpr.user=tu-github-username
gpr.token=tu-github-token
```

### 2. Usar módulos desde mavenLocal (desarrollo)

Si estás desarrollando localmente:

```bash
# En repo-principal
cd ../repo-principal
./scripts/publish-local.sh

# Volver a este proyecto
cd ../repo-pais-C
./gradlew clean build
```

## 🏃 Ejecutar

```bash
./gradlew assembleDebug
./gradlew installDebug
```

O desde Android Studio: Run > Run 'app'

## 📱 Características

- **HomeScreen**: Pantalla principal con ejemplos de uso de componentes compartidos
- **ProfileScreen**: Perfil de usuario usando `UserModel`
- **SplashScreen**: Pantalla de inicio personalizada
- **Navigation**: Navegación con Jetpack Compose Navigation

## 🔗 Repositorios Relacionados

- [repo-principal](../repo-principal) - Módulos compartidos
- [repo-pais-A](../repo-pais-A) - App Argentina 🇦🇷
- [repo-pais-B](../repo-pais-B) - App Brasil 🇧🇷

## 📄 License

MIT License
