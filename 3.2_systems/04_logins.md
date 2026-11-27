# Detecting Suspicious Activity

## Objective

Learn about **detective security controls**.

---Isto é usado para saber se alguem tentou entrar em minha conta e quantas vezes tentou e falhou

## Step 1 – View authentication logs

```bash
sudo journalctl -u ssh -n --no-pager

```

## Step 2 – Search for login attempts
```bash
sudo journalctl -u ssh --no-pager | grep -1 'failed password'
```

## Step 3 – View recent logins
```bash
sudo journalctl -u ssh --no-pager | grep -1 'accepted' | tail -n 10

## Questions
- What information appears in authentication logs? it didn't appear anything.
- Why are logs important in cybersecurity?it is , we can see how many times someone tried to logging our account
- What might indicate suspicious activity?
many attenpts 

## Deliverables
Include screenshots of:<img width="1600" height="1200" alt="image" src="https://github.com/user-attachments/assets/fdd4d2cb-f395-4a99-80b1-d821492ddda2" />

- authentication logs
- failed login search results
