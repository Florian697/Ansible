# Role: gather_versions

This role gathers version information for various applications on specified hosts and writes the results to a CSV file.

## Tasks
- Collects OS and application versions.
- Handles missing or unreachable hosts.
- Generates a summary file in CSV format.

## Usage
Include this role in your playbook:

```yaml
- name: Gather versions
  hosts: "{{ hosts_to_deploy }}"
  become: yes
  roles:
    - gather_versions
