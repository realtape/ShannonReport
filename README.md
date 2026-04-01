# Shannon Event Conversion Dashboard

## Outputs

- `shannon_event_conversion_dashboard.html`  
  Executive dashboard for Shannon with event performance, funnel metrics, and attribution status.
- `shannon_event_conversion_data.json`  
  Structured metrics snapshot generated from source documents in `C:\Users\Usuario\Downloads`.

## Rebuild Once

```powershell
python C:\Users\Usuario\Documents\NetWebMedia\tools\build_shannon_event_dashboard.py
```

## Continuous Autonomous Updates

Run a local loop every 15 minutes:

```powershell
powershell -ExecutionPolicy Bypass -File C:\Users\Usuario\Documents\NetWebMedia\tools\run_shannon_dashboard_autoupdate.ps1 -IntervalMinutes 15
```

Install startup scheduled task:

```powershell
powershell -ExecutionPolicy Bypass -File C:\Users\Usuario\Documents\NetWebMedia\tools\install_shannon_dashboard_task.ps1 -IntervalMinutes 15
```
