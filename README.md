# Infinite Fic Forge

**Infinite Fic Forge (IFF)** — настольное приложение для Windows, предназначенное для создания и ведения длинных художественных проектов с помощью ИИ: генерации глав, планирования сюжета, живой Canon Wiki, отслеживания прогрессии, иллюстраций, резервных копий и переносимых проектов.

Этот репозиторий — **официальная публичная страница бинарных релизов IFF**. Исходная разработка ведётся отдельно.

## Скачать

Откройте раздел **Releases** справа и скачайте последнюю стабильную версию.

Для большинства пользователей:

- `InfiniteFicForge-<version>-Setup.exe` — обычный установщик Windows.
- `InfiniteFicForge-<version>-portable-windows-x64.zip` — portable-версия без установки.

Каждый релиз также содержит SHA-256 checksums и служебные файлы для встроенного обновления.

## Что умеет IFF

- Генерация длинных глав с планированием, проходами критика и возобновляемыми checkpoint'ами.
- Project Canon Wiki, Reference Canon / Setting Packs и provenance фактов.
- Планирование Saga / Arc и поддержка систем прогрессии.
- OpenAI, Claude, Venice, OpenAI-compatible и локальные AI endpoint'ы.
- Генерация иллюстраций с visual continuity и semantic QA.
- Crash Recovery, Backup / Restore и переносимость книг через `.iff-project`.
- Русский и английский интерфейс, встроенный Help Center и демонстрационная книга.

## API-провайдеры и локальные данные

IFF **не включает подписку на ИИ-сервисы**. Пользователь подключает собственный поддерживаемый API-провайдер или локальный endpoint. Использование внешних API может тарифицироваться самим провайдером.

Книги и проектные данные хранятся локально в выбранной пользователем папке Library. API-ключи сохраняются через системное хранилище учётных данных ОС там, где это поддерживается.

## Ограничение версии 1.0

Интерфейс IFF поддерживает русский и английский языки, однако generation pipeline версии 1.0 пока остаётся Russian-first. В английских проектах более поздние AI-сгенерированные главы или обновления Canon иногда могут переключаться на русский. Полноценный project-level `content_language` запланирован после 1.0.

## Предупреждение Windows

Первые публичные сборки пока не подписаны code-signing сертификатом, поэтому Windows SmartScreen может показать предупреждение о неизвестном издателе. Подпись бинарников планируется как отдельный этап hardening.

## Каналы обновлений

- `latest.json` — последний стабильный релиз.
- `beta.json` — последняя доступная сборка, включая prerelease-версии.

IFF сверяет размер файла и SHA-256 перед установкой загруженного обновления.

---

## English

**Infinite Fic Forge (IFF)** is a Windows desktop app for building and maintaining long-running AI-assisted fiction projects: chapter generation, story planning, a living Canon Wiki, progression tracking, illustrations, backups and portable project export.

This repository is the **official public binary distribution home** for IFF. Open **Releases** and download the newest stable version.

For most users:

- `InfiniteFicForge-<version>-Setup.exe` — standard Windows installer.
- `InfiniteFicForge-<version>-portable-windows-x64.zip` — portable build without installation.

IFF does not include an AI subscription. Users connect their own supported provider or local endpoint. Books and project data are stored locally in the selected Library directory.

The 1.0 desktop UI supports Russian and English, but the generation pipeline is still Russian-first; full per-project content-language enforcement is planned after 1.0.
