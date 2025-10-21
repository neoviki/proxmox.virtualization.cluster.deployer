# Proxmox Automation Utilities

**Repository Name:** `proxmox.virtualization.cluster.deployer`

This project provides a set of scripts (utilities) to simplify and automate administrative tasks on a Proxmox server. Proxmox is an open-source virtualization platform for managing virtual machines (VMs) and containers, offering solution for deploying, managing, and backing up virtualized environments.

These scripts provide an easy to use interface for common Proxmox operations such as creating, deleting, exporting, importing, and restarting VMs. They also allow you to enable or disable the Proxmox web-based GUI and configure serial console access.

---

## What is Proxmox?

Proxmox VE (Virtual Environment) is an open-source virtualization platform that supports:

* **KVM:** Full virtualization for VMs
* **LXC:** Lightweight container-based virtualization

Proxmox allows centralized management of virtualized infrastructure, with features including:

* Built-in web interface for managing VMs, containers, storage, and networks
* High availability and live migration support
* Flexible resource allocation for CPU, memory, and storage

Proxmox is widely used in both enterprise and personal environments for building scalable virtualized infrastructures.

---

## Utilities

### 1. `delete.vm`

Deletes a specified virtual machine (VM) from the Proxmox server.

**Usage:**

```bash
$ ./delete.vm <vm_id>
```

* `<vm_id>`: The ID of the VM you wish to delete.

---

### 2. `export.vm`

Exports a VM to a specified file format for backup or transfer.

**Usage:**

```bash
$ ./export.vm <vm_id> <export_path>
```

* `<vm_id>`: The ID of the VM to export
* `<export_path>`: Destination path for the exported VM

---

### 3. `gui.disable`

Disables the Proxmox web-based GUI.

**Usage:**

```bash
$ ./gui.disable
```

---

### 4. `gui.enable`

Enables the Proxmox web-based GUI.

**Usage:**

```bash
$ ./gui.enable
```

---

### 5. `import.vm`

Imports a previously exported VM into the Proxmox server.

**Usage:**

```bash
$ ./import.vm <import_path>
```

* `<import_path>`: Path to the VM export file

---

### 6. `restart.hard`

Performs a hard restart of the Proxmox server, rebooting all services.

**Usage:**

```bash
$ ./restart.hard
```

---

### 7. `restart`

Restarts a specific VM on the Proxmox server.

**Usage:**

```bash
$ ./restart <vm_id>
```

* `<vm_id>`: The ID of the VM to restart

---

### 8. `serial.connect`

Establishes a serial connection to a specified VM for console access.

**Usage:**

```bash
$ ./serial.connect <vm_id>
```

* `<vm_id>`: The ID of the VM to connect to

---

### 9. `serial.enable`

Enables serial console access for a specified VM.

**Usage:**

```bash
$ ./serial.enable <vm_id>
```

* `<vm_id>`: The ID of the VM to enable console access for

---

## Prerequisites

* A running Proxmox server
* Appropriate permissions to interact with Proxmox services
* The VM IDs or paths required for specific operations

---

## References

[Proxmox Official Website](https://www.proxmox.com/en/)

