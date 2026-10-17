# Claude tooling (kendi makinende kur)

Bu repo üçüncü taraf kod veya otomatik hook içermez. Araçları yerelde, tek seferlik kur.

| Araç | Kurulum | Not |
|---|---|---|
| task-observer | `npx skills add rebelytics/one-skill-to-rule-them-all --skill task-observer -g` | Aktivasyon için `CLAUDE.md` bloğu gerekir. Yeni oturumda doğrula. Lisans: CC BY 4.0. |
| claude-mem ("Claude-man" varsayıldı) | `npx claude-mem install` | `npm i -g` kullanma (hook'ları kurmaz). Viewer: localhost:37777. Doğru araç olduğunu teyit et. |
| Headroom | `pip install "headroom-ai[all]"` sonra `headroom wrap claude` | %60–95 tasarruf iddiası üreticiden. Kendi verinde `headroom perf` ile ölç. |
| claude-code-setup | `/plugin install claude-code-setup@claude-plugins-official` | Öneriler için claude-automation-recommender skill'ini çalıştır. |
| OmniRoute | github.com/diegosouzapw/OmniRoute (npm/Docker) | Çalışan sunucu + sağlayıcı anahtarı gerekir. Dashboard localhost:20128. Kullanım: `export ANTHROPIC_BASE_URL=http://localhost:20128`. Sağlayıcı şartlarını kontrol et (Antigravity üzerinden Claude erişimi yasaklı olarak işaretli). |

Kurulum sırası: task-observer, Headroom, claude-code-setup. claude-mem ve OmniRoute'u ancak ihtiyaç doğarsa ekle; ikisi de ek bakım yükü getirir.
