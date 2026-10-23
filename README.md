# ToysGroup — Progettazione e analisi di un database vendite (MySQL)

Progettazione da zero di un database relazionale per **ToysGroup**, azienda di giocattoli, e analisi delle vendite tramite query SQL. Esercitazione finale del modulo di database (MySQL) del corso Data Analyst EPICODE.

**Autrice:** Carol Pagano · **Strumento:** MySQL Workbench

---

## Cosa contiene il progetto

- **Progettazione del modello dati**: modello concettuale (E-R) e modello logico relazionale, con tre tabelle — `Product`, `Region` e `Sales` (la tabella transazionale, collegata alle altre due tramite chiavi esterne).
- **Creazione e popolamento** del database in MySQL (DDL e INSERT).
- **Query di analisi** sulle vendite: fatturato e quantità per prodotto, per categoria, per stato e per anno; prodotti mai venduti; verifica dell'unicità delle chiavi primarie.

## Tecniche SQL usate

JOIN tra più tabelle · aggregazioni con `GROUP BY` e `HAVING` · subquery · `CASE WHEN` · funzioni di data (`YEAR`) · `LEFT JOIN` per individuare i prodotti senza vendite.

## File

| File | Contenuto |
|---|---|
| `ToysGroup.sql` | Script completo: creazione, popolamento e query di analisi (commentato) |
| `ToysGroup_Modello Concettuale (ER).png` | Modello concettuale (entità-relazione) |
| `ToysGroup_Modello Logico Relazionale.png` | Modello logico relazionale |
| `Risposte alla Traccia.pdf` | Le risposte svolte, con i risultati delle query |
| `Traccia.pdf` | Traccia originale dell'esercitazione |

## Come eseguire

In MySQL Workbench, apri ed esegui `ToysGroup.sql`. Lo script ricrea il database da zero a ogni esecuzione (`DROP DATABASE IF EXISTS`), quindi è ripetibile senza errori.
