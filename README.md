# NEXAGEN - FastQ Quality Control & Trimming Tool

NEXAGEN FastQ Quality Control Software, NGS (Next-Generation Sequencing) məlumatlarının təmizlənməsi, filtrlənməsi və keyfiyyət analizi üçün hazırlanmış yüngül və interaktiv Python tətbiqidir.

Tətbiq həm kod üzərindən, həm də rahat **Qrafik İstifadəçi İnterfeysi (GUI)** vasitəsilə FastQ fayllarını emal etməyə və ətraflı HTML hesabatları yaratmağa imkan verir.

---

## 🛠 Features (Xüsusiyyətlər)

* **FastQ Parsing:** Ham FastQ fayllarını sürətli və effektiv şəkildə oxuyur.
* **Quality Filtering & Trimming:**
  * Aşağı keyfiyyətli bazların Phred score (Q-score) göstəricisinə əsasən kəsilməsi (Trimming).
  * Müəyyən olunmuş minimum uzunluqdan kısa oxunuşların kənarlaşdırılması.
  * Naməlum bazaların (`N`) sayına görə filtrləmə.
* **Interactive GUI (Tkinter):** Parametrləri daxil etmək və fayl seçmək üçün istifadəçi dostu pəncərə.
* **Comprehensive HTML QC Report:**
  * Ümumi oxunuş (Reads) və baza (Bases) sayı.
  * **Q20** və **Q30** faiz göstəriciləri.
  * **Per-Base Sequence Quality** (Nukleotid pozisiyalarına görə Phred balı) qrafiki.
  * **GC Content Distribution** qrafiki.

---

## 🚀 Quraşdırma və İşə Salınma

### 1. Tələblər (Prerequisites)
Proqramı işlətmək üçün sisteminizdə **Python 3.8+** və aşağıdakı kitabxanalar quraşdırılmalıdır:

```bash
pip install matplotlib
