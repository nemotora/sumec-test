Projde každý submodul v hlavním repozitáři a uvnitř něj spustí zadaný příkaz

```
git submodule foreach git pull origin main
```

V každém submodulu se provede `git pull` na vzdálenou větev `main`, čímž se stáhnou a aplikují nejnovější změny z jeho repozitáře.

Pokud aktualizujete submoduly a chcete tyto změny uložit i v hlavním repozitáři, je potřeba commitnout nové reference následujícím příkazem

```
git add .
git commit -m "Aktualizace všech submodulů na nejnovější verzi"
git push origin hlavni-vetev
```