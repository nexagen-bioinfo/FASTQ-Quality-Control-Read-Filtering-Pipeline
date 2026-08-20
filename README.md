readme_content = """# NEXAGEN - FastQ Quality Control & Trimming Tool

NEXAGEN FastQ Quality Control Software, NGS (Next-Generation Sequencing) məlumatlarının təmizlənməsi, filtrlənməsi və keyfiyyət analizi üçün hazırlanmış yüngül və interaktiv Python tətbiqidir.

Tətbiq həm kod üzərindən, həm də rahat **Qrafik İstifadəçi İnterfeysi (GUI)** vasitəsilə FastQ fayllarını emal etməyə və ətraflı HTML hesabatları yaratmağa imkan verir.

---

## 🛠 Features (Xüsusiyyətlər)

* **FastQ Parsing:** Ham FastQ fayllarını sürətli və effektiv şəkildə oxuyur.
* **Quality Filtering & Trimming:**
  * Aşağı keyfiyyətli bazların Phred score (Q-score) göstəricisinə əsasən kəsilməsi (Trimming).
  * Müəyyən olunmuş minimum uzunluqdan qısa oxunuşların kənarlaşdırılması.
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
2. Tətbiqin İşə Salınması
Kodu terminal və ya Jupyter Notebook üzərindən icra edə bilərsiniz:

Bash
python app.py
Açılan pəncərədən .fastq faylınızı seçin, parametrləri (Q-score, min uzunluq) təyin edin və "Analizi Başlat" düyməsini sıxın.

📊 Çıxış Faylları (Output)
Analiz tamamlandıqdan sonra output/ qovluğunda aşağıdakı fayllar yaradılır:

clean_reads.fastq — Filtrlənmiş və təmizlənmiş NGS oxunuşları.

qc_report.html — Vizual qrafiklər və metrikalar daxil olan interaktiv hesabat faylı.

📝 Qeyd (Phred Quality Score)
Q20 (1 in 100 error rate) — Minimum qəbul edilən keyfiyyət həddi (99% dəqiqlik).

Q30 (1 in 1000 error rate) — Yüksək dəqiqlikli NGS analizi üçün standart hədd (99.9% dəqiqlik).
"""

with open("README.md", "w", encoding="utf-8") as f:
f.write(readme_content)

print("✅ 'README.md' faylı uğurla yaradıldı!")


Fayl yarandıqdan sonra GitHub-a göndərmək üçün terminalda bu 3 əmri işə salın:

```bash
git add README.md
git commit -m "Add README documentation"
git push
