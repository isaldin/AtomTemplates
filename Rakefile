namespace "templates" do
  install_dir = File.expand_path("~/Library/Developer/Xcode/Templates/File Templates/Atom")
  src_dir = File.expand_path("../AtomTemplates", __FILE__)

  desc "Install Atom templates"
  task :install do
    if File.exists? install_dir
      raise "RAKE TASK FAILED: Atom templates are already installed at #{install_dir}"
    else
      mkdir_p install_dir
      cp_r src_dir, install_dir
    end
  end

  desc "Uninstall Atom templates"
  task :uninstall do
    rm_rf install_dir
  end
end
