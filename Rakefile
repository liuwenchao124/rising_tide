#!/usr/bin/env ruby
require_relative 'models'

# exec command: rake task_name
# example: rake check_server_health

task :check_server_health do
  hostname = $hosts.keys
  servers = Helpers::CheckServerHealth.new(hostname)
  servers.check_process
  servers.check_disk_space
  servers.check_net_traffic
end

task :rearrange_upload_to_download do
  Rearrange.upload_to_download
end

task :clear_download do
  Rearrange.clear_download
end


