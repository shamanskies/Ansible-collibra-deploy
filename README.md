# Ansible Role: Collibra Platform Self-Hosted

Installs and configures CPSH on RHEL 8 or 9 servers. This is the application portion only. 

### Features

- [x] System memory and ulimits check
- [x] PostgreSQL installation from public repo
- [x] Automated Push and installation of CPSH
- [x] Start of Console and Agent services
- [ ] Configuration of environment on console

## Host Variables

The Following variables are needed for the silentInstall.json template. (see /inventory/host_vars):

    # inventory/host_vars/<node>.yml
    "repositoryMemory": {{ repository_memory }},
    "dgcMinMemory": {{ dgc_min_memory }},
    "dgcMaxMemory": {{ dgc_max_memory }},
    
    "componentSet":
  
