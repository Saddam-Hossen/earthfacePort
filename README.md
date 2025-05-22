---

# 🌍 **earthfacePort**

A centralized list of local ports and deployed URLs for Earthface applications.

<details>
<summary>📋 Click to expand app list</summary>

| 🚀 Application        | 🔌 Frontend Port | 🔧 Backend Ports                   | 🌐 Website URL                                                |
| --------------------- | ---------------- | ---------------------------------- | ------------------------------------------------------------- |
| **Device Management** | `3079`           | —                                  | *No URL provided*                                             |
| **Attendance System** | `3082`           | `3080` (User), `3081` (Attendance) | [earthface.biz/login](https://earthface.biz/login)            |
| **IT Training App**   | `3084`           | `3083`                             | [studentpanel.sohojit.com](https://studentpanel.sohojit.com/) |
| **Test Angular**      | `3085`           | `3086`                             | *No URL provided*                                             |
| **HRM Training App**  | `3087`           | `3088`                             | *No URL provided*                                             |

</details>

---

> ✅ **Tips**:
>
> * Click the dropdown above to collapse or expand the table.
> * You can replace the “No URL provided” placeholders as your deployments go live.
> * Keep this file in sync with your actual deployment to avoid confusion.




---

### 🔐 Command:

```bash
sudo ufw allow 3079
```

### ✅ Meaning of Each Part:

| Part    | Explanation                                                                                                                      |
| ------- | -------------------------------------------------------------------------------------------------------------------------------- |
| `sudo`  | Runs the command with **superuser (admin)** privileges. Required for firewall changes.                                           |
| `ufw`   | Stands for **Uncomplicated Firewall**, a user-friendly interface for managing firewall rules on Linux (typically Ubuntu/Debian). |
| `allow` | Tells the firewall to **allow traffic** through a specific port.                                                                 |
| `3079`  | The **port number** to be opened for incoming traffic.                                                                           |

---


### 🔍 Optional: Allow Specific Protocol or IP  . I am using it.

* Allow only **TCP**:

  ```bash
  sudo ufw allow 3079/tcp
  ```
* Allow only from a specific IP (e.g. only from your office IP):

  ```bash
  sudo ufw allow from 203.0.113.1 to any port 3079
  ```

---

### 📋 Check Status:

To see current firewall rules:

```bash
sudo ufw status
```

---



